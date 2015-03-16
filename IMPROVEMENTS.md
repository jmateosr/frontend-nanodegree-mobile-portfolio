##Optimize PageSpeed Insights score
- Unfied, minified and inlined CSS
- Added the WebFont as a fontface into the stylesheet
- Minified JS
- Set the size of some images
- Set the JS as async them to avoid render-blocking
- Optimized all the images (and created a pizzeria thumbnail on index)
- Delete commentaries

##60fps (modifications from lines 253 to 278)
- Calculate the calculation of the scrollTop outside the loop
- Reduced the amount of sliding pizzas generated from 200 to 20
- Replace querySelector/querySelectorAll by getElementById/getElementsByClassName to improve load speed

##Resizing pizza under 5ms (modifications from lines 213 to 220)
- Moved determineDX() call into changePizzaSizes() (outside the loop) and select only the first .randomPizzaContainer
- Calculate newwidth outside the loop and select only the first .randomPizzaContainer
- Create elemPizza var to find all the .randomPizzaContainer outside the loop and then apply the newwidth.