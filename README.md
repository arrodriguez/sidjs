## SidJS
### SidJS is a lightweight JavaScript library used to load JavaScript scripts and CSS stylesheets on demand. It increases AJAX applications performance by loading resources when they're needed.

AJAX applications make heavy use of JavaScript and stylesheets. Loading the resources only when and where they are needed makes web applications load faster and perform better.
Lazy loading is a technique that increases web applications performance by loading the resources on the fly.
SidJS is a lightweight JavaScript library that allows one to include JavaScript scripts and CSS stylesheets on demand. It supports callbacks tied to the loading process to guarantee that the resources you're loading are available when you need them.

### Methods
There are two methods available:
```javascript
Sid.js(urls [, callback]
```
##### Loads a list of JavaScript files and calls the specified callback when they're available
```javascript
Sid.css(urls [, callback])
```
##### Includes a list of stylesheets and calls the specified callback once they become available
Example
```javascript
Sid.js("my-module.js", function() {
        myModule.init();
        });
```
##### The urls parameter can be an URL or an array of URLs.

Note: this library is open source software distributed under the terms of the BSD license

