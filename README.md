# jQuery.redirect
A simple HTTP POST and GET Redirection Plugin for jQuery

* Easy to use
* GET and POST requests
* Works in any WebBrowser
* Supports nested objects and arrays


## Usage:
 ```javascript
/**
 * jQuery Redirect
 * @param {string} url - Url of the redirection
 * @param {Object} values - (optional) An object with the data to send. If not present will look for values as QueryString in the target url.
 * @param {string} method - (optional) The HTTP verb can be GET or POST (defaults to POST)
 * @param {string} target - (optional) The target of the form. If you set "_blank" will open the url in a new window.
 */
$.redirect(url, [values, [method, [target]]])

/* Example */
var params = { 
       "FormInputKey1": "KeyValue1",
       "FormInputKey2": "KeyValue2"
             }
 $.redirect("/myController/myMethod", params, "post", "_self")
 ```

## How does it work?
The function jQuery.redirect will create a form and populate it with the data (it supports nested values).

## How to install the plugin:
Just download jquery.rediect.js and include it in your html after jquery.js

 ```html
 <html>
 <head>
     <!-- other headers -->
     <script src="jquery-XXX.js"></script>
     <script src="jquery.redirect.js"></script>
 </head>
 <body>
     <!-- your content -->
 </body>
 </html>

