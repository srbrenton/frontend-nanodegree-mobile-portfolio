frontend-nanodegree-mobile-portfolio
====================================
Instructions
------------
The source for this project is on GitHub, direct your browser to:

<https://github.com/srbrenton/frontend-nanodegree-mobile-portfolio/>

To interact with this project, direct your browser to:

<http://srbrenton.github.io/frontend-nanodegree-mobile-portfolio/>

See [Cam's Pizzeria](http://srbrenton.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html)
for wildly moving pizzas when you scroll the Pizza Menu page

Modifications to index.html for PageSpeed evaluation
----------------------------------------------------
* Used Macintosh "GraphicConverter X" from lemkesoft.com to optimize these images:
    
    BEFORE:<br>
14K  img/profilepic.jpg

    AFTER:<br>
5.9K img/profilepic.jpg

    BEFORE:<br>
2.3M views/images/pizzeria.jpg

    AFTER:<br>
23K  views/images/pizzeria.jpg<br>
    4.8K views/images/pizzathumb.jpg

* Adjusted bit depth (number of colors) and natural/display size as suggested in:
<https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization>
* Read contents of css/style.css into &lt;style&gt; block in index.html
* Moved contents of index.html &lt;script&gt; block into js/fromindex.js
* Added media="print" to css/print.css link
* Added async attribute to &lt;script&gt; tags in index.html

views/js/main.js modifications
------------------------------
* moved several calls for DOM elements outside the loops used to update their attribute values
* refactored 'pizza size' slider to eliminate meaningless code per the video lesson
* added a simple 'animate' function to limit scroll updates to once per frame
* refactored background pizza sine movement using translate calls to update the pizzas in their own layer
* added 'will-change: translate' css attribute and value to .mover class
