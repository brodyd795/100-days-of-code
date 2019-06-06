# 100 Days Of Code - Log

### Day 18: June 5, 2019

**Today's Progress**: Continued working on user authentication

**Thoughts**: I've got the full auth0 sample page working on my site, though it's still throwing a few errors that I don't quite understand yet. Next step will be figuring out how auth0 maintains user sessions and how I can save/retrieve data during a given user's session. 

**Link to work**: No link for this yet, but I've basically added the code from the auth0 sample to my existing code from yesterday.

### Day 17: June 4, 2019

**Today's Progress**: Configured prototype of user authentication login button

**Thoughts**: I started off assuming that I'd build my own simple authentication system using a JSON object of usernames and passwords, given the low security needs of the project. However, I decided it'd be better to learn how to integrate a real auth system, so I went with auth0 and got started on their site (https://auth0.com/) with their QuickStart tutorial. I downloaded the zip file, followed the instructions, and ran it – worked just fine. The troubles came when I tried to integrate it into my own system. So, I took a step back and created a new bare-bones project with just a login button. It turned out that loading Auth0 via dependencies neglected to include a crucial part of the package that is available through their CDN. Once I figured that out and included it as a src, it worked like a charm. Finally, I made sure it all worked with a view engine. User auth -- like many other things -- turns out to be much more complicated than I initially imagined. But hey – the challenge is good!

**Link to work**: No link available yet, but here's the main chunk of code from today (which goes along with a simple node+express setup with an index.ejs view and a simple login button):
```javascript
window.addEventListener('load', function() {
  var idToken;
  var accessToken;
  var expiresAt;
  var webAuth = new auth0.WebAuth({
    domain: 'dev-dingel.auth0.com',
    clientID: 'my-client-id',
    responseType: 'token id_token',
    scope: 'openid',
    redirectUri: window.location.href
  });

  var loginBtn = document.getElementById('btn-login');

  loginBtn.addEventListener('click', function(e) {
    e.preventDefault();
    webAuth.authorize();
  });

});

```

### Day 16: June 3, 2019

**Today's Progress**: Finished a prototype of the regex interface!

**Thoughts**: Today I separated the site from one page into four separate pages to make the code cleaner and more logical. I also incorporated all of the express.js code into the site to all for get/post requests, and importantly, I make the regex tester work on the interface and post a score to the page using express and ajax. Express is getting more intuitive now, though my understanding of the combination of express and ajax is still a bit shaky. Next steps: saving/retrieving user data, user authentication, sessions, and further styling. It's amazing how far I've come in just 16 days!

**Link to work**: http://brody.linguatorium.com:8080/

### Day 15: June 2, 2019

**Today's Progress**: Finished the regex tester!

**Thoughts**: After 3 days of work, I finally got the regex tester to work – it now takes a series of regular expressions as input (as prompted by a task description) and returns a final score based on a series of tests. Now I'll incorporate this into the site, and then comes user authentication...

**Link to work**: Can't post the code for security reasons, here is the main logic:
```javascript
module.exports = {
  testRegex: function(input, task) {
    var regexArr = input.split(/\r?\n/);
    var task = task;

    var allTests = {dictionary of tests and answers}

    var testStrings = allTests[task]["tests"];
    var resultStrings = allTests[task]["answers"];
    var pts = 0;
    var ptsPoss = testStrings.length;
    for (let i=0; i<testStrings.length; i++){
      var testString = testStrings[i];
      var resultString = resultStrings[i];

      for (let j=0; j<regexArr.length; j++){
        let regexpStr = regexArr[j];
        var regexMatch = regexpStr.replace(/s\/(.*?)\/.*?\/\w+$/, "$1");
        var regexReplace = regexpStr.replace(/s\/.*?\/(.*?)\/\w+$/, "$1");
        var regexFlags = regexpStr.replace(/s\/.*?\/.*?\/(\w*?)$/, "$1");
        var realRegex = new RegExp(regexMatch, regexFlags);
        var testString = testString.replace(realRegex, regexReplace);
      };
    if (testString == resultString) {
      pts++;
    }
    var score = (pts/ptsPoss)*100;
    score = score.toFixed(2);
    }
    console.log(pts + "/ " + ptsPoss);
    console.log("score: " + score);
    return score;
  }
};

```

### Day 14: June 1, 2019

**Today's Progress**: Continued working on logic for regex tester

**Thoughts**: Today I tried linking the Perl code into my JS code so as to not reinvent the wheel, but this doesn't seem to be a very popular method, based on the relative lack of available packages for doing so. I decided that it'd be easier to just continue writing it from scratch in JS. By the end of the day, I finally have a working regex tester! Now I need to make it test against a series of test strings and return a score, link it all up to the rest of the site, and re-work the site using views (as I said I'd do a couple of days ago). 

**Link to work**: Can't post the code for security reasons, but will post the main logic once it's done

### Day 13: May 31, 2019

**Today's Progress**: Starting working on the JS logic for testing regular expressions for accuracy in my regex site

**Thoughts**: Before I started this project, my mentor gave me his code in Perl that accomplishes basically the same task. (He told me to code the site on my own for learning purposes, but gave me the regex testing engine to get started.) After comparing how his code accomplishes the task to how I intend to do it in JS, it seems like the syntax of regular expressions in Perl lends itself to this task better than JS's syntax – interesting! I spent a lot of time dissecting his code to figure out the logic, and I started coding it in JS. Long way to go. 

**Link to work**: Can't post the code for security reasons, but will post the main logic once it's done

### Day 12: May 30, 2019

**Today's Progress**: Figured out how to do POST requests using Express.js and Node.js on my remote server

**Thoughts**: After three days of reading online documentation and doing online tutorials (and much confusion), I am finally on track to ipmlement POST requests into my regex site. One lesson I've learned througout this issue is to learn from various sources – find multiple tutorials, multiple docs, read up on stackoverflow questions on the topic, etc., and don't just rely on one "all-in-one" tutorial. Tomorrow I want to restructure my regex site a bit to incorporate EJS views rather than putting all the content on one page, and I also want to add the form elements to implement the POST requests. A rough couple of days, but it's coming together!

**Link to work**: No link available, since I was just playing around with test files, but here's the main bit of code that I put together:
```javascript
var express = require('express');
var app = express();
var bodyParser = require('body-parser');
var urlencodedParser = bodyParser.urlencoded({ extended: false});
app.set('view engine', 'ejs');
app.get('/', function(req, res){
  res.render('index');
});
app.post('/index', urlencodedParser, function(req, res) {
  console.log(req.body);
  var myString = req.body.who;
  var patt = new RegExp("Rach");
  var myMatch = patt.test(myString);
  console.log(myMatch);
  res.render('index');
})
app.listen(3000);
```

### Day 11: May 29, 2019

**Today's Progress**: Began learning about node.js/AJAX/express for sending and processing client form data on a remote server. Also started the basic layout of my Technical Documentation Page.

**Thoughts**: HTML/CSS are becoming easier and easier to implement, but this new issue of processing form data on a server and retrieving the results is a new problem that I'm not sure how to handle. AJAX seems relatively straightforward, but most of the Express tutorials I've found online work with a server created on the local machine, whereas I'm working with a remote server. Planning to continue looking into how AJAX and Express (and Node.js) interact more in the coming days, as this is crucial for the next step in my regex website project. 

**Link to work**: https://github.com/brodyd795/technicalDocumentationPage

### Day 10: May 28, 2019

**Today's Progress**: Finished authenticating my home budgeting tool!

**Thoughts**: Finally figured out that building the service for the API call is basically identical regardless of the authentication method. I successfully migrated from a client-server authentication (which isn't right for my uses) to authentication between the server and a web application (which does fit my uses). My next step might be to figure out how to most securely store and access credentials on my local machine. 

**Link to work**: https://github.com/brodyd795/accounting

### Day 9: May 27, 2019

**Today's Progress**: Continued node.js tutorial, began working on revised authentication method for my home budgeting tool

**Thoughts**: I'm rather confused about the different methods of authentication for Google APIs (e.g., client-server vs. server-web-application), but reading through the documentation and it's beginning to make more sense.

**Link to work**: https://github.com/brodyd795/accounting

### Day 8: May 26, 2019

**Today's Progress**: Continued working on the HTML/CSS/JS for my regex site, started a node.js tutorial

**Thoughts**: Starting to think about how to get users logged into the site, creating usernames/passwords, authenticating, etc. Seemed like I didn't have much of an idea about how this all works behind the scenes, so a node.js tutorial is seeming to help me to understand all of this.

**Link to work**: https://github.com/brodyd795/regex-site

### Day 7: May 25, 2019

**Today's Progress**: Started working on a website for my future students in a Computers and Language class to practice their regular expressions. HTML/CSS/JS are really coming along already!

**Thoughts**: Initially tried working with Bootstrap to make it more easily responsive, but I don't think I'm comfortable enough yet with HTML/CSS, so I stuck to plain language to practice this more before moving to Bootstrap. The interface came together pretty quickly, and now I need to work on user authentication, the db, and integrating the regular expression checker to assess my students' learning.

**Link to work**: https://github.com/brodyd795/regex-site

### Day 6: May 24, 2019

**Today's Progress**: Got closer to a final product for my product landing page

**Thoughts**: Now that the HTML and CSS look decent for the screen I'm working on, now I need to work on making it responsive.

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC

### Day 5: May 23, 2019

**Today's Progress**: Got most of the positioning figured out with CSS, worked a bit on beautifying the page

**Thoughts**: Flexbox is becoming much more intuitive. Still trying to figure out what color schemes and other styling I want to add to the page. Once this is done, I'll need to work on making it responsive for other widths and devices. 

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC

### Day 4: May 22, 2019

**Today's Progress**: Finally getting the product landing page looking right! Flexbox skills are developing nicely.

**Thoughts**: It took quite a bit of trial and error, along with reading plenty of online articles, but I'm finally getting the hang of flexbox and overall CSS positioning. Today was quite a bit of a confidence booster after the past two days. Very happy with how it's beginning to look!

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC

### Day 3: May 21, 2019

**Today's Progress**: Kept working on the CSS of the product landing page, began applying flexbox concepts

**Thoughts**: Slowly starting to understand flexbox. Still don't have much to prove for my gains in understanding the CSS, but it's getting there.

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC

### Day 2: May 20, 2019

**Today's Progress**: Re-did some of the HTML and started over on the CSS. 

**Thoughts**: Turned out that I really didn't have a firm understanding of the basics of CSS, so I went back to redo some tutorials and took some notes. Visibly, not much progress, but definitely starting to understand things better now! Here are the (very rough) notes that I took just to jog my own memory for later.

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC

-div elements take up the full width of their container unless you specify their width, and each div starts on a new 'line' since it is a block-level element, while inline elements (e.g., spans) will only take up as much space as necessary and will stay on the same line as their neighbors
-rather than setting 'width: 50px' for a div, set 'max-width: 50px' so that the browser won't set a horizontal scroll bar if the window is less than that width (e.g., on mobile devices) --> basically, just set max-width

-there are 5 positions: static, relative, fixed, absolute, and sticky
-these positions can use top, left, bottom, and right properties to specify the position, but this must be specified AFTER specifying the position
-static is the default position for all elements, and it's not affected by the TRBL properties
-relative is the position relative to an element's normal position
-fixed positions the element in a fixed location in the viewport; other elements are not affected by it's positioning
-absolute positions the elements relative to the nearest positioned ancestor
-sticky positions the element in a fixed spot only after a predetermined amount of scrolling; until this point, it is relatively positioned

-overflow lets you make text get into a scroll property rather than simply get clipped at the end of the div; this is a good idea to have

-float lets you make one element be positioned to the right/left of another elements within their mutual parent container; this is useful for having text and an image within a container where the image needs to be floated to one side of the text
-however, when an element is floated but it is larger than it's container, it will overflow (e.g., when a paragraph and image are within a div, but the image is bigger than the div); rather than setting the margins/padding specially, you can just use the clearfix hack (https://www.w3schools.com/css/css_float.asp)

-note: need to learn about border box later

-display: inline-block is very useful for navigation links - boxes that sit next to each other

-descendents: use "div p" to affect all ps within the div; use "div > p" to only select immediate p children of the div


### Day 1: May 19, 2019

**Today's Progress**: Started working on CSS for the content on my Product Landing Page project from FreeCodeCamp.com

**Thoughts:** Slowly figuring out HTML and CSS. Seems like there are sometimes several ways to structure content in HTML (e.g., links in a nav bar as list items in ul vs. separate divs/spans), but it's the layout with CSS that's still really challenging me. 

**Link to work:** https://github.com/brodyd795/productLandingPage-FCC
