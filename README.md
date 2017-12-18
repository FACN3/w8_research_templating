# Week 8 Research. Topic: Templating

## 1.(a) What is Server Side Rendering

If you make a request on server-rendered sites, the browser gets back the fully rendered HTML and displays it on the screen. If you then decide to visit a different page on the website, your browser will once again make another request for the new information. This will occur each and every time you visit a page that your browser does not have a cached version of.

It doesn’t matter if the new page only has a few items that are different than the current page, the browser will ask for the entire new page and will re-render everything from the ground up.

## (b) What is Client Side Rendering

The key difference is that if you were to click on a link the page to load more content, the browser will not make another request to the server. You are rendering items with the browser, so it will instead use JavaScript to load the new content and a templating framework/language will make sure that only the new content is rendered. Everything else will be left alone.


### Server-side pros:

   + Search engines can crawl the site for better SEO.
   + The initial page load is faster.
   + Great for static sites.

### Server-side cons:

   + Frequent server requests.
   + An overall slow page rendering.
   + Full page reloads.
   + Non-rich site interactions.

### Client-side pros:

   + Rich site interactions
   + Fast website rendering after the initial load.
   + Great for web applications.
   + Robust selection of JavaScript libraries.

### Client-side cons:

   + Low SEO if not implemented correctly.
   + Initial load might require more time.
   + In most cases, requires an external library.
