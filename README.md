#Web Performance Optimization
### Udacity Nanodegree Project 4

Link to [Frontend-Nanodegree-Mobile-Portfolio/](http://projects.jordanyong.com/frontend-nanodegree-mobile-portfolio/)



####Steps taken to achieve score above 90 on index.html on [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* Optimized Images by resizing and minifying
* Minified CSS and JS
* Move JS to end of HTML body tag
* Add async to script tag


####Pizza.html
This was an extremely difficult project for me to get under 60fps.
Only way I could get close to 60fps after trying all the other steps was to reduce the number of pizzas.


Steps taken to achieve 60fps and pizza resize under 5 ms
* 4 things the browser can animate cheaply.
Position - transform: translate(npx, npx);, Scale - transform: scale(n);, Rotate - transform: rotate(ndeg);, Opacity: 0..1;
Source: http://www.html5rocks.com/en/tutorials/speed/high-performance-animations/
* Utilized transform: scale(n);, to resize Pizzas
* Utilized transform: translateX(npx);, for pizza animation when scrolling
* Add async in JS
* Minified CSS and JS
* compressed and utilized svg formats for images
* Reduced number of pizzas
