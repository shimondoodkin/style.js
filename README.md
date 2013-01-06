style.js
========

$style.js css loader
https://github.com/shimondoodkin/style.js
(c) Shimon doodkin 2012
License: MIT

```javascript
function $style(css){
  var style = document.createElement('style');
  style.type = 'text/css';  
  if (style.styleSheet) { // IE
      style.styleSheet.cssText = css;
  } else {
      style.appendChild(document.createTextNode(css));
  }
  document.getElementsByTagName('head')[0].appendChild(style);
}
```

usage inside javascript:
-----------------------
```javascript
$style("@import url('/stylesheets/orders.css');");
$style("@import url('http://123.123.123.123:5051/stylesheets/orders.css');");
$style('.example {'+
       ' width : 90%;'+
       '  height: 90%;'+
       '  margin: 8px auto;'+
       '} '+
       //+'.item{border:1px solid lightgray;padding:10px;}'+
       '')
```
