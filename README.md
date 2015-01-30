#Web Performance Optimization
### Udacity Nanodegree Project 4

Link to [Frontend-Nanodegree-Mobile-Portfolio/](http://projects.jordanyong.com/frontend-nanodegree-mobile-portfolio/)



####index.html
Steps taken to achieve score above 90 with [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* Optimized Images by resizing and minifying
* Minified CSS and JS
* Move JS to end of HTML body tag
* Add async to script tag


####pizza.html
This was an extremely difficult project for me to get under 60fps.
Only way I could get close to 60fps after trying all the other steps was to reduce the number of pizzas.
Main concern leading to low fps was the long paint time. There were two insights that lead to long paint times by Paul Irish [Profiling Long Paint Times](http://updates.html5rocks.com/2013/02/Profiling-Long-Paint-Times-with-DevTools-Continuous-Painting-Mode)
* CSS styles: background-attachment:fixed
* Reduce the painting cost of the areas that get repainted
* CSS styles: border-radius and box-shadow

In this case I've reduced the number of moving pizzas to reduce the painting cost


Steps taken to achieve 60fps and pizza resize under 5 ms
* Utilized transform: scale(n); to resize pizzas
* Utilized transform: translateX(npx); for mocing pizzas when scrolling
* Add async in JS
* Minified CSS and JS
* compressed and utilized svg formats for images
* Reduced number of pizzas to reduce cost of areas that get repainted


Resources used throughout this project
* [Optimizing Performance](https://developers.google.com)
* [Advanced performance tooling in Chrome DevTools - Paul Irish](https://www.youtube.com/watch?v=0xx_dkv9DEY)
* [High Performance Animations](http://www.html5rocks.com/en/tutorials/speed/high-performance-animations/)
* [Resize Images](http://www.picresize.com/)
* [Compress png](https://tinypng.com/)
* [Gulp](https://gulpjs.com)
* [Profiling Long Paint Times - Paul Irish](http://updates.html5rocks.com/2013/02/Profiling-Long-Paint-Times-with-DevTools-Continuous-Painting-Mode)