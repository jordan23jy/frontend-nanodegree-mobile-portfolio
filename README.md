#Web Performance Optimization
### Udacity Nanodegree Project 4

Link to [Frontend-Nanodegree-Mobile-Portfolio/](http://projects.jordanyong.com/frontend-nanodegree-mobile-portfolio/)

Optimized sections are commented 'OPTIMIZE:' in main.js for pizza.html

####index.html
Steps taken to achieve score above 90 with [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* Optimize Images by resizing and minifying
* Minify CSS and JS
* Move JS to end of HTML body tag
* Add async to script tag


####pizza.html
Steps taken to achieve 60fps and pizza resize under 5 ms

Pizza Resize
* Move out of sizeSwitcher function out of determineDX loop (calulation only done once instead of within each loop)
* Calculate new width of pizza outside loop once, as all containers are the same

Moving Pizzas
* Determine scroll top position outside of for loop when updating updating position of moving pizzas during scroll
* Utilize style = transform: translateX, avoiding layout re-rendering
* Initial position of moving pizza is set outside of loop

General
* Add async in JS
* Minify CSS and JS
* Compress and utilized svg formats for images
* Reduce number of moving pizzas in header from 200 to 36, to reduce cost of areas that get repainted


Resources used throughout this project
* [Optimizing Performance](https://developers.google.com)
* [Advanced performance tooling in Chrome DevTools - Paul Irish](https://www.youtube.com/watch?v=0xx_dkv9DEY)
* [High Performance Animations](http://www.html5rocks.com/en/tutorials/speed/high-performance-animations/)
* [Resize Images](http://www.picresize.com/)
* [Compress png](https://tinypng.com/)
* [Gulp](https://gulpjs.com)
* [Profiling Long Paint Times - Paul Irish](http://updates.html5rocks.com/2013/02/Profiling-Long-Paint-Times-with-DevTools-Continuous-Painting-Mode)