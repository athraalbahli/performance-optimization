
# Website Performance Optimization project

* I separate the source code and production code under src and dist folders
* All production files are minified, but you can access the unminified version under src folder


## Setps to improve the website performance:

### index.html 
1. Load google font using the [web font loader] library.
2. Use async attribute with the google analytics js file to executed the file asynchronously.
3. Move the inline javascript code for google analytics in separate file and make it execute asynchronously by adding the async attribute.
4. Add media=“print” on the link tag for the print.css file so the file will not block the page rendering.
5. Compress and resize images.
6. Set the with and height of the image using css.
7. Minify html, css and js files.

### pizza.html 

1. Compress and resize images.
2. Set the with and height of the image using css.
3. Minify html, css and js files.

### main.js

1. Change “changePizzaSizes” function by placing the calculation of the new pizza width out side the “for” loop 
2. On the “DOMContentLoaded” EventListener, I set the element attribute outside the “for” loop because we only need to set to once.
3. on “updatePositions” function, I moved this line outside the loop 
```javascript
 var scrollTop = document.documentElement.scrollTop || document.body.scrollTop;alert(s);
```