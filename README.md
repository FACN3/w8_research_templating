# Week 8 Research. Topic: Templating & Serverside rendering

 
## 1.(a) What is Server Side Rendering
 
If you make a request on serverrendered sites, the browser gets back the fully rendered HTML and displays it on the screen. If you then decide to visit a different page on the website, your browser will once again make another request for the new information. This will occur each and every time you visit a page that your browser does not have a cached version of.

It doesn’t matter if the new page only has a few items that are different than the current page, the browser will ask for the entire new page and will rerender everything from the ground up.

## (b) What is Client Side Rendering

The key difference is that if you were to click on a link the page to load more content, the browser will not make another request to the server. You are rendering items with the browser, so it will instead use JavaScript to load the new content and a templating framework/language will make sure that only the new content is rendered. Everything else will be left alone.


### Serverside pros:

   + Search engines can crawl the site for better SEO.
   + The initial page load is faster.
   + Great for static sites.

### Serverside cons:

   + Frequent server requests.
   + An overall slow page rendering.
   + Full page reloads.
   + Nonrich site interactions.

### Clientside pros:

   + Rich site interactions
   + Fast website rendering after the initial load.
   + Great for web applications.
   + Robust selection of JavaScript libraries.

### Clientside cons:

   + Low SEO if not implemented correctly.
   + Initial load might require more time.
   + In most cases, requires an external library.

###### [Read More Here](https://medium.freecodecamp.org/whatexactlyisclientsiderenderingandhowsitdifferentfromserversiderenderingbd5c786b340d)


## When is it useful to use templating engine/language?
You should use a JavaScript templating engine like Handlebars.js when:


* You use a JavaScript frontend framework like Backone.js, Ember.js, and the like; most frontend JavaScript frameworks rely on templating engines
* The application’s view (the HTML page or portions of the page) will be updated frequently, especially as a result of changes to the data either from the server via a REST API or from data on the client  
* You have multiple tech stacks that depend on your data from the server and you want all the tech stacks to process the same data  
* Your application has much interactivity and it is very responsive  
* You are developing a singlepage web application with multiple views  
* You want to easily manage your HTML content; you don’t want your JavaScript code to contain important HTML markup. 


## Example of Functionality that Templating languages provide
```
{{singleVrible}}
{{object.key}} 
{{{function parameter}}}
{{{function paramOne=value  paramTwo="value"}}}  
{{{function paramOne=value  paramTwo="paramTwo" moreParams=value}}}
{{{function.subFunction params}}}
{{#unless(if not) somthing}}
{{if(condision) something}}
{{with(include) somthing in object}} // else can be use in this
{{log (just console.log) 'string' param 'string'}}
{{lookup (Loops through an array and checks if not null)}}
```
