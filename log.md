# 100 Days Of Code - Log

### Day 4: May 22, 2019

**Today's Progress**: Finally getting the product landing page looking right! Flexbox skills are developing nicely.

**Thoughts**: It took quite a bit of trial and error, along with reading plenty of online articles, but I'm finally getting the hang of flexbox and overall CSS positioning. Today was quite a bit of a confidence booster after the past two days. Very happy with how it's beginning to look!

### Day 3: May 21, 2019

**Today's Progress**: Kept working on the CSS of the product landing page, began applying flexbox concepts

**Thoughts**: Slowly starting to understand flexbox. Still don't have much to prove for my gains in understanding the CSS, but it's getting there.

### Day 2: May 20, 2019

**Today's Progress**: Re-did some of the HTML and started over on the CSS. 

**Thoughts**: Turned out that I really didn't have a firm understanding of the basics of CSS, so I went back to redo some tutorials and took some notes. Visibly, not much progress, but definitely starting to understand things better now! Here are the (very rough) notes that I took just to jog my own memory for later.

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
