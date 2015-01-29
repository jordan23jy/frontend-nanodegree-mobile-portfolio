#Web Performance Optimization
### Udacity Nanodegree Project 4

Link to [Frontend-Nanodegree-Mobile-Portfolio/](http://projects.jordanyong.com/frontend-nanodegree-mobile-portfolio/)



Steps taken to achieve score above 90 on [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* Optimized Images by resizing and minifying
* Minified CSS and JS
* Move JS to end of HTML body tag
* Add async to script tag


Steps taken to optimize main.js in pizza.html
* 4 things the browser can animate cheaply.
Position - transform: translate(npx, npx);, Scale - transform: scale(n);, Rotate - transform: rotate(ndeg);, Opacity: 0..1;
Source: http://www.html5rocks.com/en/tutorials/speed/high-performance-animations/
* Utilized transform: scale(n);, to resize Pizzas
* Utilized transform: translateX(npx);, for pizza animation when scrolling
* Add code at end of file to allow for async call in HTML

Resources used while completing the project
* Information about image optimization:
http://addyosmani.com/blog/image-optimization-tools/
* Minimize jpg file size:
http://www.jpegmini.com/
* Minimize png file size:
http://pngquant.org/
* CSS Minifier
http://cssminifier.com/
* JavaScript Minifier
http://javascript-minifier.com/
* Optimizing Performance https://developers.google.com/web/fundamentals/performance/
* Analyzing the Critical Rendering Path https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html
* Optimizing the Critical Rendering Path https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html
* Avoiding Rendering Blocking CSS https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html
* Optimizing JavaScript https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html
* Piazza https://piazza.com/ Project 4 discussions
