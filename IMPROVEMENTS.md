##Optimize PageSpeed Insights score
- Unfied, minified and inlined CSS
- Added the WebFont as a fontface into the stylesheet
- Minified JS
- Set the size of some images
- Set the JS as async them to avoid render-blocking
- Optimized all the images (and created a pizzeria thumbnail on index)
- Delete commentaries

##60fps 
- Calculate the phaseInt outside the loop
- Limit the number of pizzas generated when loading the page
- Replace querySelector/querySelectorAll by getElementById/getElementsByClassName to improve load speed