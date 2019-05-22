# Performance

## Keys to performance optimization Part 1

### Frontend

1. Critical render path
2. Optimized code
3. Progressive Web App

### File Transfer

1. Minimize Files

   a. JS minification:

   - Uglify JS

   b. Image file Tips:

   - Use the correct file format for the job (jpg, png, gif, svg)
     PNG for transparency
   - GIF for animations
   - JPG for colorful images
   - Reduce PNG with TinyPNG
   - Reduce JPG with JPEG-optimizer
   - Try to use simple illustrations over highly detailed images
   - Always use lower JPG quality (30-60%)
   - Resize images for sizes that will be displayed
   - Display different sized images for different backgrounds
   - Use CDNs like imigx
   - Remove image metadata

2) Minimize Delivery

3) Critical Render Path

   a. DOM

   b. CSSOM

   c. Render Tree

   d. Layout

   e. Paint

   <hr />

- HTML
  - Load style tag in the <head>
  - Load script right before </body>
- CSS
  - Only load whatever is needed.
  - Above the fold loading
  - Media attributes
  - Less specificity
- Javascript
  - Load scripts asynchronously
  - Defer loading of scripts
  - Minimize DOM manipulation
  - Avoid long running Javascript
  - <b>DOMContentLoaded</b>: an event listener that is fired when the DOM has fully loaded
  - <b>Async</b>: scripts will load in any random order
  - <b>Defer</b>: (Not 100% supported) scripts will not load until the DOM has loaded
  - \*If JS events change any part of the page, it causes a redraw of the render tree and it forces us to go through the Layout and Paint processes again and again.\*

### Backend

1. CDNs
2. Caching
3. Load Balancing
4. DB Scaling
5. GZIP

<hr />

## Keys to performance optimization Part 2

<hr />

#### Key Notes

- Average website should load within 2sec.

#### Resources

Image file formats

https://99designs.com/blog/tips/image-file-types/

https://pageweight.imgix.com/

https://www.sitepoint.com/gif-png-jpg-which-one-to-use/

Media Queries

https://www.verexif.com/en/

https://css-tricks.com/snippets/css/media-queries-for-standard-devices/

http://www.bsidestudios.com/blog/media-queries-common-sizes-cheat-sheet

Delivery

https://stackoverflow.com/questions/985431/max-parallel-http-connections-in-a-browser

Async & Defer

https://stackoverflow.com/questions/10808109/script-tag-async-defer

Speed Testing

https://developers.google.com/speed/pagespeed/insights/

google lighthouse plugin chrome

https://tools.pingdom.com/

https://www.webpagetest.org/
