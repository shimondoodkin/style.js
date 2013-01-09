$style.js - a tiny css loader
========
It enables to load stylesheets dynamicaly from javascript.

I used it to build single .js file embedable apps.

https://github.com/shimondoodkin/style.js

(c) Shimon Doodkin 2012

License: MIT

usage inside javascript:

```javascript
$style.url('/stylesheets/orders.css');
$style.url('http://123.123.123.123:5051/stylesheets/orders.css';
$style('.example {'+
       ' width : 90%;'+
       '  height: 90%;'+
       '  margin: 8px auto;'+
       '} '+
       //+'.item{border:1px solid lightgray;padding:10px;}'+
       '')
```

I have tested it with ie6 ie7 ie8 ie9 - it works with them. it does not work with ie5.5.

Also CSS that contain @import directive do not work in ie8 or less.

It works well in many other browsers


Related:

$script.js - a small async javascript loader: https://github.com/ded/script.js
