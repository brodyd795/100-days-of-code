# 100 Days Of Code - Log

### Day 76: August 8, 2019

**Today's Progress**: Continued with SQLite – made successful connection!

**Thoughts**: 

**Link to work**: https://github.com/brodyd795/ling120-course-website

### Day 75: August 7, 2019

**Today's Progress**: Continued with SQLite

**Thoughts**: Today I was able to log the output of the SQLite error onto my page, and I see that the app is unable to find the table. I'm confident that the table exists, yet I'm finding no resources online to hint at why the table can't be found. Disheartening to not have made much of any progress, but just need to keep pushing through and problem solve to knock this bug out. Hopefully tomorrow will shed more light.

**Link to work**: https://github.com/brodyd795/ling120-course-website

### Day 74: August 6, 2019

**Today's Progress**: Began working with SQLite to create an attendance tracking tool for my course website

**Thoughts**: Started looking through tutorials and trying to create a sample database and open it from Node.js. Turning out to be a more difficult problem than I imagined, for some reason. Can't get a connection to the database, but will continue trying tomorrow. One accomplishment is having drawn out the design of the tool in terms of the UI and GET/POST requests, which was important and very helpful to conceptualize the project.

**Link to work**: https://github.com/brodyd795/ling120-course-website

### Day 73: August 5, 2019

**Today's Progress**: Portfolio is done, up and running!

**Thoughts**: Couldn't figure out why the "stretched-link" class in Bootstrap wouldn't work. Learned that it was due to the version of Bootstrap I was using, so I switched to the latest version through CDN and fixed that problem. Unfortunately, that also removed some borders on a few elements, but I was able to override that with !important. Added the final bit of content to my page, and now it's ready for the world to see! (Obviously still have some things I'll improve eventually, but I'm happy with this product for now.)

**Link to work**: http://brody.linguatorium.com/

### Day 72: August 4, 2019

**Today's Progress**: Basically done with my portfolio!

**Thoughts**: Added my email functionality to my personal site, made the navbar a bit prettier, and worked on making final tweaks to styling. Important to set margin and padding on the body to 0. One tiny thing to fix tomorrow!

**Link to work**: http://brody.linguatorium.com

### Day 71: August 3, 2019

**Today's Progress**: Continued styling portfolio page

**Thoughts**: Happy to be nearly finished with styling my page. Got my picture lined up right and found a few other things, including the navbar, to style up a bit. Sometimes seems like a never-ending process. Getting there!

**Link to work**: http://brody.linguatorium.com

### Day 70: August 2, 2019

**Today's Progress**: Continued styling portfolio page

**Thoughts**: Realized there was a fair bit of styling that I wanted done still, so I'll have to spend a few days on this. Struggling today with lining up a picture of myself with some text, so I'll start with that tomorrow. 

**Link to work**: http://brody.linguatorium.com

### Day 69: August 1, 2019

**Today's Progress**: Got personal site up at correct URL

**Thoughts**: Was able to get files onto my server easily enough, but moving things around so that my html file was rendered instead of pug files proved a bit more challenging. Shows the importance of keeping the same protocol across an entire site, because it would have been rough translating my entire html file into pug. Also saw the importance of trying to anticipate the scope of the project before starting, because my file system looks a bit odd now with subdirectories named 'brody' to indicate my personal site amongst the regex site. Got it all figured out though!

**Link to work**: http://brody.linguatorium.com

### Day 68: July 31, 2019

**Today's Progress**: Continued styling portfolio page – closer to done!

**Thoughts**: Got my navbar looking a bit nicer on the correct side of the page, fixed some odd scrolling (margins/padding issue), moved some px measurements to responsive measurements, and more. Getting closer to a final product! Tomorrow I'll focus on getting this thing online, but that'll require some reconfiguration in my regex site code since the regex site is at brody.linguatorium.com where I want my personal site to appear. Happy with what I've got so far!

**Link to work**: https://github.com/brodyd795/personal-website

### Day 67: July 30, 2019

**Today's Progress**: Continued styling portfolio page

**Thoughts**: Finished getting the rest of my old code from my previous version of the portfolio site onto the new version where I've been making simple styling changes and making it more responsive. Getting more familiar with techniques for making the page responsive, like staying away from px and instead using em/rem/vw/vh/etc. Keep on chugging.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 66: July 29, 2019

**Today's Progress**: Fixed bugs in old code – weather app and accounting app

**Thoughts**: I sometimes wonder how other people store credentials to their code, because any time that I change a password, I have to remember what apps it pertains to and have to manually update the credentials within the app. Is there a better way to manage all of this? A couple of my app stopped working a while ago since I had changed a password, so I got those up and running again, I fixed a bug in the accounting app that allows it to work effectively with each new month, and I made the weather app a bit more secure by storing my credentials outside of the code. Not much heavy lifting today, but definitely necessary work.

**Link to work**: https://github.com/brodyd795/weather-app AND https://github.com/brodyd795/accounting

### Day 65: July 27, 2019

**Today's Progress**: Finished modifying JS file for work

**Thoughts**: Looked into potential bug sent by supervisor, only to dismiss. Then wrote some instructions for my future self to follow along with so I can recreate the code adjustments with future videos. Happy with the final result!

**Link to work**: Uncertain if the code is open source, so unable to share

### Day 64: July 26, 2019

**Today's Progress**: Worked on modifying JS file for work, nearly finished and sent product to supervisor

**Thoughts**: Decided to continue working on the JS code to change the desired features. The code from a 3rd-party software is for an embedded video with automated quiz questions inside an LMS system. Through heavy use of the Chrome dev tools and trial/error, I was able to find ways to (1) remove a button that allows students to skip the quiz (you'd think the option to remove this button would be available in the software that creates the code...) and then adjust the margins, and (2) disable all rewind/fast forward/pausing abilities on the video. I was unable to find a way to disable pausing entirely since the video needs to call the pause whenever a quiz question appears, so I changed the keycode from SPACE to P, which won't be problematic since it's a multiple-choice quiz. Very happy with the final result, especially given the fact that it was minified code and with HTML embedded in JS functions. 

**Link to work**: Uncertain if the code is open source, so unable to share

### Day 63: July 25, 2019

**Today's Progress**: Worked on debugging a minified file for work, continued styling on portfolio site

**Thoughts**: Tried to make a feature change on a minified JS file for a work-related task today, but without luck. I was able to track down the primary bit of code to delete the feature, but it seems that the code is connected to other places in the code that would take more time to track down that isn't worth the time. Good to have the experience working with minified files. Definitely helps to keep others from modifying the code. Also kept working on my portfolio's styling. Fixed an issue with a breakpoint and started looking into how to make font sizes responsive, which doesn't seem like an easy task, oddly enough.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 62: July 24, 2019

**Today's Progress**: Continued with styling on portfolio site

**Thoughts**: Starting fresh was a good idea. I'm really noticing some major styling issues that were causing non-responsiveness, and I've solved many issues just on the landing page. Still working with font sizes and trying to make everything responsive to all devices, but I also think that this is something that I'll need to work on over time. So, just trying to get it as responsive as I can in the moment, then move on to another element. With styling, I've found that a good night's sleep can do wonders, as with much other code. Read something similar to this on Twitter today with the great #100DaysOfCode community there.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 61: July 23, 2019

**Today's Progress**: Continued with styling on portfolio site

**Thoughts**: Kept working with the styling in Bootstrap from scratch. Getting some good reminders about the Bootstrap fundamentals and flexbox. Also seeing the importance of not using px for font sizes but rather em and rem. 

**Link to work**: https://github.com/brodyd795/personal-website

### Day 60: July 22, 2019

**Today's Progress**: Continued with styling on portfolio site

**Thoughts**: Struggling to make my site responsive, as I'm sure everyone does. Even with bootstrap, it's rather difficult, especially on the landing page. I thought that it may have to do with some of the layout of the elements (the overlay of the background image on the landing page), and I decided that it may be best to start fresh and work my way down the page, making sure everything is responsive as I go. So, I got started on that journey, with promising results so far.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 59: July 21, 2019

**Today's Progress**: Added logging feature to regex site, continued working on setting up new computer

**Thoughts**: Looking down the road, I imagine students asking me for help on their regex assignment, me asking them what they've tried recently, and them not having a log. So, I quickly added the functionality in JS to log their score and the timestamp along with their attempt with every submit. Surprising how easy this was! I also managed to get the GUI on my computer to work after configuring the ethernet connection with dhclient, only to find that no terminal could be found in the GUI (to my knowledge). After installing gnome-terminal, the GUI no longer appears at all. More debugging to do.

**Link to work**: http://brody.linguatorium.com/

### Day 58: July 20, 2019

**Today's Progress**: Continued styling of portfolio site, worked on setting up new-to-me computer

**Thoughts**: I kept moving forward with my portfolio styling, and I'm beginning to wonder if I should start from scratch with Bootstrap, keeping the old version in front of me. I think this might make my code cleaner and more standardized, and it might help make things more responsive in the end. I'm still on the fence about this, but it might be worth dedicating an hour or two sometime to see if this would help. On another note, a family member gave me an old Dell with CentOS on it, so I started working on getting the GUI set up, though to no avail yet. Still having trouble getting it to recognize an internet connection.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 57: July 19, 2019

**Today's Progress**: Continued styling of portolio site

**Thoughts**: Slowly but surely getting things on my portfolio site looking the way I want them. Styling continues to be the hardest part of software development for me, but it's getting much better over time (judging by my progress over 57 days). Sometimes the Bootstrap defaults throw me off, so it takes a bit of debugging to figure out why, for example, the padding doesn't act the way I want it to. The Chrome dev tools have helped in these endeavors. 

**Link to work**: https://github.com/brodyd795/personal-website

### Day 56: July 18, 2019

**Today's Progress**: Updated styling of my course website

**Thoughts**: Made some pretty simple styling changes to the course website, but then again, they were simple. If I were to restart the HTML and CSS of the project, I'd do things completely differently, probably with Bootstrap. Given that I designed the site while I was learning the very basics of HTML/CSS, the site is not responsive in the least, so this is something I might fix someday when I have some spare time. However, the purpose of the site doesn't necessitate responsiveness (though it'd be nice), since my students will be using the site in a laboratory setting using predictable computers and browsers. Always keeping the usage in mind!

**Link to work**: http://brody.linguatorium.com/ and https://github.com/brodyd795/ling120-course-website

### Day 55: July 17, 2019

**Today's Progress**: Pre-filled dropdown field, trimmed whitespace from user input, cleaned code

**Thoughts**: Productive hour of coding! I fixed the pre-fill dropdown field (way easier than I thought...), trimmed the whitespace from user input to prevent errors from occurring, and went through some code and added comments and removed old code. One of those feel-good days.

**Link to work**: http://brody.linguatorium.com/

### Day 54: July 16, 2019

**Today's Progress**: Pre-filled the code field, working on dropdown field

**Thoughts**: Got to work with Pug templates again today (it's been a while!). Had an interesting bug where the value attribute of a textarea would appear in the Chrome inspector tool but not in the actual window. Tried copy/pasting into a plain HTML document (same result) and looking at the source code in the browser. Finally dawned on me that perhaps textareas don't have a value attribute – and they don't! Very easy fix to render the variable between the textarea tags. However, I'm struggling to implement the pre-filling in the dropdown menu. I've tried a few solutions online, but to no avail yet. I'm thinking that JS in the Pug template might lead me to the right answer. We'll see tomorrow!

**Link to work**: http://brody.linguatorium.com/

### Day 53: July 14, 2019

**Today's Progress**: Began implementing pre-fill on form fields for user convenience

**Thoughts**: Wasn't sure how to pre-fill form fields in the Pug template engine, but it seems like it'll be pretty easy and similar to pure HTML. I've worked out the logic for how/when to prefill by writing it in plain English first, and that seemed to be a pretty good strategy that I'll continue using in the future. About halfway done, I think.

**Link to work**: http://brody.linguatorium.com/

### Day 52: July 13, 2019

**Today's Progress**: Worked on testing for quality assurance of course website

**Thoughts**: Worked with a colleague to determine lingering flaws and areas for improvement in the code of my course website. He suggested that I pre-fill some form fields with the user's previous response for user convenience, so I began considering how this could be accomplished. Will begin working to implement this feature tomorrow. Also beginning to think about style changes to make the site more appealing.

**Link to work**: http://brody.linguatorium.com/

### Day 51: July 12, 2019

**Today's Progress**: Added feature to log all user submissions to course website

**Thoughts**: Decided to add a feature to log all submissions that my students make on their assignments, thinking it would just take a few minutes to add. Naturally, it took a few hours, but I got to practice writing a bit more JS. I also began to wonder... is restarting the server after changing JS files really necessary, or could I just RESTART the Forever command? Might try out the next time I modify the JS code.

**Link to work**: http://brody.linguatorium.com/

### Day 50: July 11, 2019

**Today's Progress**: Removed old files, secured credentials, tried adding "120/" to URL

**Thoughts**: Didn't add much new code today, but I took care of some smaller TODO items like removing old files and adding credentials to the .env file so I could push the rest of the files to github. I also tried adding "120/" into the URL so that I can reserve "brody.linguatorium.com" for my personal website later on, but without success. Will continue to work on this. I also want to log user submissions on the server, so will work on that tomorrow. 

**Link to work**: http://brody.linguatorium.com/

### Day 49: July 10, 2019

**Today's Progress**: Finished feature of choosing a course for blackbox, ran into bugs, resolved bugs

**Thoughts**: Interesting how many issues can only be resolved by restarting the server. The nodemailer call that I was running wouldn't update until I restarted the server, and at that point, the login call stopped working. I realized that I had left the quotation marks around some process.env.VARIABLES from when I was debugging and included the variables hard-coded. Naturally, removing the quotes didn't work until I restarted the server. Now it's all up and running! Tomorrow I'll rework the URL so that the site comes up at brody.linguatorium.com/120 rather than just brody.linguatorium.com. 

**Link to work**: http://brody.linguatorium.com/

### Day 48: July 8, 2019

**Today's Progress**: Fixed bugs on course website, began additional feature of choosing course for blackbox

**Thoughts**: I had three bugs that I couldn't figure out how to resolve: (1) the logout page would direct me to an undefined domain, (2) a .json data file couldn't be found, and (3) occasionally when trying to start the site the app couldn't find the domain credentials in the .env file. It turned out that all three errors were due to starting the app with "forever" in the wrong directory, as the app couldn't find the .env file or the .json file. Once I had this resolved, the site worked perfectly. I've also begun adding a field to the blackbox page to select which course the student belongs to and adding that field into the subject line of an email sent to me anonymously, but the email call is not updating (keeps sending emails with the old subject line to one email address regardless of what I put in those parameters). Will resolve tomorrow hopefully. 

**Link to work**: http://brody.linguatorium.com/

### Day 47: July 7, 2019

**Today's Progress**: Worked on fixing bug from trying to add additional security measures

**Thoughts**: While trying to add the additional security measures, I managed to insert a bug somewhere in the program such that my email function no longer works. The POST request goes through, and no errors are written to the error log, yet the email is not sent. Spent a few hours looking into this today, and will hopefully resolve by tomorrow.

**Link to work**: http://brody.linguatorium.com/

### Day 46: July 6, 2019

**Today's Progress**: Continued working on footer, fixed bugs in course website, began adding extra security feature to course website

**Thoughts**: Still can't get the footer to align flush with the bottom of the page. Have tried margins, absolute/relative positioning, flexbox, etc. Nothing seems to align it correctly, so still investigating. Maybe I'll have more progress on this tomorrow. On the bright side, I managed to fix the bugs on my course website so that the whole site runs smoothly! The program was trying to print to the console even after I had disconnected from the ssh, causing the site to crash. I also (finally) added the whole project to github, so I can have better version control. Finally, I also began adding some further security measures with the dotenv package, though still working on making this perform properly. Productive day!

**Link to work**: https://github.com/brodyd795/personal-website, http://brody.linguatorium.com/

### Day 45: July 5, 2019

**Today's Progress**: Finished Contact section on portfolio site, began footer

**Thoughts**: After enough messing around with forms and trying to center things the way I wanted them, I've finally got a working Contact section with a nice collabsible form. Moved into working on the footer, and can't seem to find a way to make a footer with absolute position in Bootstrap. So many examples of fixed or sticky footers, but can't find hardly anything on absolute positioning. Perhaps I'm searching for the wrong term? Will further investigate tomorrow.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 44: July 4, 2019

**Today's Progress**: Began adding a Contact section to my portfolio site

**Thoughts**: Taking a while to figure out how forms work in Bootstrap (seems like nearly every feature can be translated into Bootstrap, assuming you know the right classes to add!), but slowly making progress. Hoping to complete the Contact section by tomorrow. Also got the Social icons looking nice!

**Link to work**: https://github.com/brodyd795/personal-website

### Day 43: July 3, 2019

**Today's Progress**: Enabled firewalld, removed port number from URL, worked on fixing bugs on server

**Thoughts**: Enabling firewalld was actually quite simple, contrary to what I expected. I also successfully removed the port number from most of the website by removing it from app.js and the Auth0 dashboard, but a bug came up with the port number still wanting to appear in the /logout route. Spent a while trying to figure this out, plus the fact that the website crashes when I try to access a new page on the website. So, more debugging tomorrow.

**Link to work**: Unfortunately, the website is down at the moment while I work on these bugs.

### Day 42: July 2, 2019

**Today's Progress**: Fixed a bug in my server configs and began pushing a new feature to my course website

**Thoughts**: I've learned in the past to read through multiple solutions to a problem online (reading to the end) before trying any code in the terminal to fix a bug, so things went much smoother this time than some other times in the past. Found that the kdump service was being allocated "auto" memory, so I edited the config to a particular amount of memory, updated the configs to the boot directory, restarted the server and my node app, and it's working! Then I worked on pushing the Black Box feature to my website (finally), and I've learned that I need a far better method of maintaining development/production versions so I can easily push to production.

**Link to work**: None available for the server work, and course website update coming soon!

### Day 41: July 1, 2019

**Today's Progress**: Worked on server configurations after scheduled maintenance

**Thoughts**: There was scheduled maintenance done on my server that hosts my course website, and it appears that some configs were changed that resulted in the website going down. Started looking into how to fix the errors (Kdump service not allocated memory), but there's a lot I don't know and several possible solutions online that I'll work on trying out tomorrow.

**Link to work**: None available, given that I was working in the terminal on my server

### Day 40: June 30, 2019

**Today's Progress**: Continued making tweaks to different sections on portfolio site, looked into MySQL

**Thoughts**: This site is really coming along! I'm glad to have learned bootstrap for this project – I seemed impossible at first for some reason (maybe I was going about it wrong?), but now it seems very helpful. I still feel like CSS is the hardest part of putting a website together, but that's coming along as well. Perhaps within a week or two I'll have this finished! On a random note, I started looking into MySQL in order to add an Attendance page to my course website. Trying to figure out whether SQL or a Google Sheet would be better/simpler (as I already have a good attendance tool in an Excel sheet). 

**Link to work**: https://github.com/brodyd795/personal-website

### Day 39: June 29, 2019

**Today's Progress**: Added Contact section to portolio site with font-awesome social media icons

**Thoughts**: Once again, Bootstrap felt 'right' for this section. However, while font-awesome seemed easy to integrate, I'm having a hard time getting them to size the way I want with the right font and background colors. Will keep looking into the CSS for this.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 38: June 28, 2019

**Today's Progress**: Added Projects section to my portfolio site

**Thoughts**: This was another section where Bootstrap was perfect. Found the Cards utility on W3Schools, and got that easily added to my site. Started working on customizing it with CSS.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 37: June 27, 2019

**Today's Progress**: Added About section to my portfolio site

**Thoughts**: It seems like Bootstraps grid system is designed for some features more than others. (Should a given page use Bootstrap for some sections, and not for other sections where it doesn't fit?) This section lent itself to Bootstrap much more than the main landing section, so it was nice to see how quickly/easily it came together. Slowly but surely Bootstrap is coming in handy!

**Link to work**: https://github.com/brodyd795/personal-website

### Day 36: June 26, 2019

**Today's Progress**: Added typeit.js functionality to main portfolio site page, began designing my About section

**Thoughts**: After experimenting with CSS, vanilla JS, etc., I found the TypeIt.js module for adding an animated typing effect to text. It works SO well. Goes to show how much value there is in searching for the right thing – a module vs. pure CSS, etc. Also began designing my About section on paper and thinking about how I could incorporate this within Bootstrap so that it's responsive. 

**Link to work**: https://github.com/brodyd795/personal-website

### Day 35: June 25, 2019

**Today's Progress**: Got a functioning timeline on my portfolio site

**Thoughts**: After much messing around, I finally found a timeline template that fits my site well, and I was able to start customizing it within bootstrap. I've learned that I need to search only for templates/guides on incorporating features using the framework that I've chosen, otherwise they simply won't work.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 34: June 24, 2019

**Today's Progress**: Continued working on portfolio website

**Thoughts**: Another relatively unproductive day working with Bootstrap. Finding it impossible to assemble a basic timeline while Bootstrap is still linked to the page, but I've used Bootstrap for everything thus far. Have looked for a way to remove default Bootstrap settings from a particular element, but can't seem to make that work either. Will need to do some more digging on this.

**Link to work**: Coming soon!

### Day 33: June 23, 2019

**Today's Progress**: Continued working on portfolio website

**Thoughts**: Having trouble getting bootstrap to place elements where I want them to go. Just seems like there are so many conflicts between CSS, CSS defaults, and Bootstrap defaults, and I hardly know where to look to find what to change. Pushing forward...

**Link to work**: Coming soon!

### Day 32: June 21, 2019

**Today's Progress**: Finished adding new functionality to my accounting app

**Thoughts**: Now the app will add a new sheet on the first day of the month, duplicate the default sheet and rename it for the new month, and then continue with adding new transactions. So happy with the final product! Also (finally) took a few minutes to learn about "git clone" and pushing/pulling from the repo from different machines.

**Link to work**: https://github.com/brodyd795/accounting

### Day 32: June 20, 2019

**Today's Progress**: Added "New Month" functionality to my accounting app

**Thoughts**: I decided to take a break from web dev for a bit and cross off some items on my TODO list for my accounting app. Previously, I had to add a new sheet to my Google Spreadsheet for each new month and copy/paste the default layout. Spending a while learning how the API works in detail, but making great progress. Should be finished by tomorrow.

**Link to work**: https://github.com/brodyd795/accounting

### Day 31: June 19, 2019

**Today's Progress**: Continued working with Bootstrap on personal website

**Thoughts**: Working with Bootstrap is getting a bit better, though still struggling to figure out how the default styles differ from using raw CSS. Finding more and more online resources to help me along with Bootstrap, which is very helpful.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 30: June 18, 2019

**Today's Progress**: Restarted personal website using Bootstrap

**Thoughts**: Decided to give Bootstrap a try given its popularity in the field. Struggling most with figuring out what the new default styles are and how I can work around them, such as how to make the navbar fixed using Bootstrap. A few more days with this, and I imagine I'll begin getting the hang of it.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 29: June 17, 2019

**Today's Progress**: Began designing personal portfolio website

**Thoughts**: There seem to be so many options when beginning to design a website that it's hard to choose. Still struggling with the basic CSS – I imagine that it will just take bulding many websites to eventually become comfortable with it. At least now I feel like I know where to look and what to look for when I need a particular functionality.

**Link to work**: https://github.com/brodyd795/personal-website

### Day 28: June 16, 2019

**Today's Progress**: Added Black Box functionality to Regex site

**Thoughts**: Found the very user-friendly Nodemailer module for sending emails in JS. Super easy to incorporate into my regex site for a Black Box functionality (where students can send an anonymous message to my email). Pug templates made it pretty easy to add the new page to the site as well.

**Link to work**: Will take some time soon to push the updated/new files to the server

### Day 27: June 15, 2019

**Today's Progress**: Finished the Technical Documentation Page

**Thoughts**: I had the Technical Documentation Page basically finished, but without content, so I added the content to it today, and it's looking pretty good! Since the topic is regular expressions, I might add it as an additional resource for my students when they're learning regex with my regex site next semester.

**Link to work**: Need to get better about pushing/committing to github.... link coming soon!

### Day 26: June 14, 2019

**Today's Progress**: Worked on fixing a bug in my accounting app, added some content to my Technical Documentation Page

**Thoughts**: Crontab is so finnicky about permissions. The environment that it runs in is different from that of the IDE, and therefore it interprets paths and permissions differently. I've detected the bug, and now working on figuring out why Crontab isn't able to open a particular file.

**Link to work**: No link yet, but hopefully I'll have it tomorrow for my Technical Documentation Page!

### Day 25: June 13, 2019

**Today's Progress**: Got the regex site online and partially eliminated the issue of the port number in the URL

**Thoughts**: Had a relative help me edit the config files on my server to add a reverse proxy (using proxy_pass) in Nginx to pass requests to the port number to a URL. Took us quite a while, but eventually figured out that (1) Nginx was expecting Ipv4 instead of the Ipv6 that we were passing to it (or was it the reverse?). It only took one additional parameter in one line of code to fix that issue. (2) SELinux was preventing the server from rendering the html files (I think?), and I'm in the process of fixing that all up. I have very little experience with servers and configs, so this is all very new to me. Learning, though!

**Link to work**: http://brody.linguatorium.com/

### Day 24: June 12, 2019

**Today's Progress**: Continued working on styling, made some progress, especially on the navbar

**Thoughts**: Happy to say that the navbar is mostly done and has most of the functionality that I originally intended for it to have. Choosing a color scheme can be frustrating, and still haven't found a website for choosing a website-wide color scheme, but will continue looking. Now to add the content to the page...

**Link to work**: https://github.com/brodyd795/technicalDocumentationPage

### Day 23: June 10, 2019

**Today's Progress**: Started working on more styling of my technical documentation page, including the navigation bar

**Thoughts**: CSS is beginning to show its complexity, once again. I'd like to make a sidenav bar that opens/closes and is responsive to different device widths, but not sure how just yet. 

**Link to work**: https://github.com/brodyd795/technicalDocumentationPage

### Day 22: June 9, 2019

**Today's Progress**: Got my regex site online!

**Thoughts**: So excited after today's progress. I fixed the last major styling issues, added some error handling, got everything put on my remote server, fixed the bugs that accompanied that step (mostly old versions of npm and node), and configured the auth system to accept the new domain. It's working! Just a few more bugs to work out before the new semester for my students to use it.

**Link to work**: http://brody.linguatorium.com:3000/

### Day 21: June 8, 2019

**Today's Progress**: Finished the authentication system, make great progress on templates (Big day!)

**Thoughts**: Today's progress was quite satisfying. I finally got the authentication system working (Woo!), I completely shifted over from the EJS to PUG templates, and I'm finally working on error handling for once I can release this project to the wild. I'm so excited! Oh, I also realized there was a bug in my budgeting app, so I fixed that and committed to github. 

**Link to work**: Regex site will be posted by tomorrow! Link to budgeting app update: https://github.com/brodyd795/accounting

### Day 20: June 7, 2019

**Today's Progress**: Continued working on user authentication and changing templating engine

**Thoughts**: User authentication is getting closer, though I had quite a shift involved after I realized I'd need to choose between the EJS templates and the PUG templates that the new auth package was using. I've decided to go with the PUG templates, because the EJS ones were causing quite a few difficulties and PUG seemed easier to manage. This is the second time that I've chosen the wrong type of tutorial while working on a project, so I definitely need to keep this mistake in mind for the future to save time/energy. Templating is seeming pretty useful – I wonder how often it's used in the "real world"? Got closer to a working veresion of the auth system by the end of the day.

**Link to work**: Still no link available... hopefully tomorrow!

### Day 19: June 6, 2019

**Today's Progress**: Continued working on user authentication

**Thoughts**: I realized today that I was using the sample authentication package from the "single web page" application type, while I needed the "regular web application". So, I began moving in this direction, and was able to make the sample package function on my site by the end of the day, though lots more work needs to be put in to make it mesh with my content.

**Link to work**: No link for this yet, but coming soon!

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
