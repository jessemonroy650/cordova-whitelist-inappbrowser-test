# cordova-whitelist-inappbrowser-test #
Date: 2015-12-15<br>
Last Update: 2015-12-15


----

## The App ##
This App compiles for iOS, Android, and Windows. It excercises the main `whitelist` elements - `<access (...) />`,`<allow-intent (...) />`, `<allow-navigate (...) />`, `CSP` and `ATS`. The App has four (4) files, seven (7) plugins, and nine (9) icons. It uses no *splash screens*.

1. index.html - body and view of the application, required
2. config.xml - App configuration, required
3. zepto-1.1.6.js - a jquery equivalent, but lighter weight

- [cordova-plugin-device](https://www.npmjs.com/package/cordova-plugin-device) - used to collect device information
- [cordova-plugin-inappbrowser](https://www.npmjs.com/package/cordova-plugin-inappbrowser) - **to be tested**
- [cordova-plugin-network-information](https://www.npmjs.com/package/cordova-plugin-network-information) - used to report network availability
- [cordova-plugin-whitelist](https://www.npmjs.com/package/cordova-plugin-whitelist) - **to be tested**

## External Files ##

The directive `<access (...) />` is the bottom filter. Everything eventually goes through `access`.

**Loads an external image an internet server.**<br>
- http://codesnippets.altervista.org/examples/phonegap/images/cordova-whitelist-example.png - image

**`CSP` external CSS from an internet server.**<br>
- http://codesnippets.altervista.org/examples/phonegap/images/cordova-whitelist-example.css - css


**window.open(url,"_self")**<br>
- http://cordova.apache.org/blog/
- requires `<allow-intent (...) />`

**window.open(url,"_system")**<br>
- http://cordova.apache.org/blog/
- requires `<allow-intent (...) />`

**window.open(url,"_blank")**<br>
- http://cordova.apache.org/blog/
- requires `<allow-intent (...) />`
