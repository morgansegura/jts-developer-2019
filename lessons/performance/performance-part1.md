# Keys to performance optimization (Part 1)

### <b>Frontend</b>

1. Critical render path
2. Optimized code
3. Progressive Web App

### <b>File Transfer</b>

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

### <b>Backend</b>

1. CDNs
2. Caching
3. Load Balancing
4. DB Scaling
5. GZIP

<hr />

##### Key Notes

- Average website should load within 2sec.

## Resources

<b>Image file formats</b>

- https://99designs.com/blog/tips/image-file-types/

- https://pageweight.imgix.com/

- https://www.sitepoint.com/gif-png-jpg-which-one-to-use/

<b>Media Queries</b>

- https://www.verexif.com/en/

- https://css-tricks.com/snippets/css/media-queries-for-standard-devices/

- http://www.bsidestudios.com/blog/media-queries-common-sizes-cheat-sheet

<b>Delivery</b>

- https://stackoverflow.com/questions/985431/max-parallel-http-connections-in-a-browser

<b>Async & Defer</b>

https://stackoverflow.com/questions/10808109/script-tag-async-defer

<b>Speed Testing</b>

- https://developers.google.com/speed/pagespeed/insights/

- google lighthouse plugin chrome

- https://tools.pingdom.com/

- https://www.webpagetest.org/

<b>Prefetching</b>

https://css-tricks.com/prefetching-preloading-prebrowsing/

<b>Dev Tools:</b>

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#activities" target="_blank">View main thread activities in a table</a> to sort activities based on which ones took up the most time.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#fps" target="_blank">Analyze frames per second (FPS)</a> to measure whether your animations truly run smoothly.

- <a href="https://developers.google.com/web/updates/2017/11/devtools-release-notes#perf-monitor" target="_blank">Monitor CPU usage, JS heap size, DOM nodes, layouts per second, and more</a> in real-time with the Performance Monitor.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#screenshots" target="_blank">Capture screenshots while recording</a> to play back exactly how the page looked while the page loaded, or an animation fired, and so on.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#interactions" target="_blank">View interactions</a> to quickly identify what happened on a page after a user interacted with it.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#scrolling-performance-issues" target="_blank">Find scroll performance issues in real-time</a> by highlighting the page whenever a potentially problematic listener fires.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#paint-flashing" target="_blank">View paint events in real-time</a> to identify costly paint events that may be harming the performance of your animations.

- <a href="https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/reference#main" target="_blank">View main thread activity</a> to view every event that occurred on the main thread while you were recording.

<b>Other Resources:</b>

- http://optimizilla.com/

- https://tools.pingdom.com/

- https://www.thinkwithgoogle.com/feature/mobile/

- https://developers.google.com/web/tools/lighthouse/

- http://websitespeedranker.com/

- https://pageweight.imgix.com/

- https://developers.google.com/speed/pagespeed/insights/

- https://passmarked.com/

- https://images.guide/

- https://www.crazyegg.com/blog/image-editing-tools/

<b>Additional image manipulation tools:</b>

<a href="https://www.xnview.com/en/xnconvert/" target="_blank">XNConvert:</a> This free, cross-platform tool can handle batched images, and performs resizing, optimization, and other transforms.
<a href="https://imageoptim.com/mac" target="_blank">ImageOptim:</a> This free tool is available for Mac and as an online service, and is specifically aimed at optimizing images for speed, including metadata removal (discussed above).
<a href="https://itunes.apple.com/us/app/resizeit/id416280139?mt=12" target="_blank">ResizeIt:</a> A Mac-only desktop product that lets you change the size of multiple images simultaneously, and can convert file formats at the same time.
<a href="http://www.picresize.com/" target="_blank">PicResize:</a> One of several good browser-based tools that gives you lots of options for cropping, rotating, resizing, adding effects to, and converting images.
<a href="https://www.gimp.org/" target="_blank">Gimp:</a> This ever-popular cross-platform tool just gets better with age. Powerful and flexible, Gimp lets you perform a wide variety of image manipulation tasks including, of course, resizing.

<b>HHTP / 2</b>

- https://developers.google.com/web/fundamentals/performance/http2/
