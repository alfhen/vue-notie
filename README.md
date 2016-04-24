# vue-notie
A Vue.js plugin wrapper for the awesome Notie.js https://github.com/jaredreich/notie

## Installation

Install through npm

``` bash
npm install vue-notie --save

```

Include in ```<body>``` after loading Vue and it will automatically hook into Vue
``` html
<script src="/node_modules/vue-notie/src/vue-notie.js'"></script>

<!-- don't forget to add the notie.js stylesheet  -->

<link rel="stylesheet" href="/node_modules/notie/dist/notie.css">
 ```

Or do it the cool way and load it in your ```main.js/app.js```

``` javascript
// Require dependencies
var Vue = require('vue');
var VueNotie = require('vue-notie');
// Tell Vue to use the plugin
Vue.use(VueNotie);

```
Don't forget to import the css or sass in your stylesheet compilation
``` scss
@import "notie/notie.scss";
```

### Usage
The pluging makes the normal notie.js module accessible through calling ```this.$notie```
###### Example
``` javascript
// From some method in one of your Vue components
this.$notie.alert(1, 'Hello world!', 3);
// This will create a green alert box with the text Hello World! lasting for 3 seconds.
```
For more Examples go and read the Notie.js documenation: https://github.com/jaredreich/notie

Thanks for using the plugin, I am happy to accept feedback/pull requests, don not forget to star The Notie.js repo!

Happy Coding! :D
