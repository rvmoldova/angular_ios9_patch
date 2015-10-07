
# Angular ios9 ui webview patch

##### Just install it via Bower

```
bower install angular_ios9_patch --save
```

 This patch works around iOS9 UIWebView regression that causes infinite digest
 errors in Angular.

 The patch can be applied to Angular 1.2.0 – 1.4.5. Newer versions of Angular
 have the workaround baked in.

 To apply this patch load/bundle this file with your application and add a
 dependency on the "ngIOS9UIWebViewPatch" module to your main app module.

 For example:

 ```
 angular.module('myApp', ['ngRoute'])`
 ```

 becomes

 ```
 angular.module('myApp', ['ngRoute', 'ngIOS9UIWebViewPatch'])
 ```


 More info:
 - https://openradar.appspot.com/22186109
 - https://github.com/angular/angular.js/issues/12241
 - https://github.com/driftyco/ionic/issues/4082
 - This plugin it's not mine, i just registered it to bower for easy instalation


 @license AngularJS
 (c) 2010-2015 Google, Inc. http://angularjs.org
 License: MIT
