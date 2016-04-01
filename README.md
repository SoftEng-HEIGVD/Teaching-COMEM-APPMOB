# COMEM APPMOB

> Course on mobile application development.



## Slides

See the [slides directory](slides).



## Links

* [Repo to develop the Citizen Engagement mobile application](https://github.com/SoftEng-HEIGVD/Teaching-HEIGVD-CM_APPMOB-2016-CitizenEngagement)
* [Repo with the completed skeleton application for the Citizen Engagement mobile application](https://github.com/SoftEng-HEIGVD/Teaching-HEIGVD-CM_APPMOB-2016-SkeletonApp)

If you want to use the reference implementation of the Citizen Engagement API rather than your own:

* [Documentation for the reference implementation of the Citizen Engagement API](https://polar-brook-7624.herokuapp.com)
* [Repo of the Express reference implementation](https://github.com/SoftEng-HEIGVD/Teaching-HEIGVD-CM_WEBS-2015-Labo-Express-Impl)
* [Repo of the API documentation for the reference implementation](https://github.com/SoftEng-HEIGVD/Teaching-HEIGVD-CM_WEBS-2015-Labo-Doc-Impl)



## Resources

* [Ionic Installation](http://ionicframework.com/getting-started/)
* [Ionic Documentation](http://ionicframework.com/docs/)

* [AngularJS](https://angularjs.org)
* [AngularJS Developer Guide](https://docs.angularjs.org/guide)
* [AngularJS API Reference](https://docs.angularjs.org/api)

* [Angular UI Router](https://github.com/angular-ui/ui-router)
* [Angular UI Router Guide](https://github.com/angular-ui/ui-router/wiki)
* [Angular UI Router API Reference](http://angular-ui.github.io/ui-router/site/#/api/ui.router)

* [Mapbox](https://www.mapbox.com)
* [Angular Leaflet Directive for Mapbox](https://github.com/tombatossals/angular-leaflet-directive)
* [Mapbox Javascript Library](https://www.mapbox.com/mapbox.js/api/v2.4.0/)

* [Cordova Camera Plugin](https://github.com/apache/cordova-plugin-camera)

* [qimg](https://github.com/SoftEng-HEIGVD/qimg)
* [qimg API Reference](http://softeng-heigvd.github.io/qimg/)



## Lab Delivery

**Delivery date:** April 18th at noon.

You are asked to provide:

* The Citizen Engagement mobile application, with the following requirements:
  * It must use geolocation.
  * It must use [Mapbox](https://www.mapbox.com).
  * It must use the camera (works only on physical devices).
* The appropriate configuration to run your application in both development and production mode.
* A user guide or presentation page for the application. You can choose from the following options (one is enough):
  * You can present the application in the README of the GitHub repository for the application (if you forked the [starting repository](https://github.com/SoftEng-HEIGVD/Teaching-HEIGVD-CM_APPMOB-2016-CitizenEngagement), get rid of the original setup instructions and replace them with your presentation).
  * You can upload your application to a store (e.g. Google Play), and write the presentation page as you would for a real application.
  * You can use any other presentation tool but your presentation page **must** be available online.
* *Optional:* A webcast demonstrating usage of the mobile application. This is not mandatory but may improve your grade if you did not fulfill all the other requirements.

**How to Deliver**

Each group must send an e-mail to `simon.oulevay [at] heig-vd.ch` with the following information:

* Who is in your group.
* The link to the GitHub repository of your Citizen Engagement mobile application.
* The link to the user guide or presentation page for the application (if it's not in the README of the repository).
* The link to the webcast for the application (if you made one).
* The configuration files (e.g. `config/development.json` and `config/production.json`) used to develop and deploy your application.



## Known Issues

* [Ionic View App Issue #10: Upload doesn't seem to be updating JS or CSS files](https://github.com/driftyco/ionic-view-issues/issues/10)

  If you are using the Ionic View App to develop your mobile application on iOS,
  be aware that sometimes uploading is not enough to refresh your code on the device.
  You might need to stop your app (swipe down with three fingers), clear app data,
  and restart the Ionic View App (double tap on home button and close Ionic View App).
  Then you can re-download your app and it should be the latest version.

* Sass compilation issues

  If `gulp-sass` fails to install with compilation issues when you run `npm install`,
  and you do not plan on writing CSS with Sass, comment the following line in `gulpfile.js`:

      //var sass = require('gulp-sass');

  And *remove* the `gulp-sass` dependency from your `package.json` file (you cannot use comments in JSON):

      "gulp-sass": "^2.0.4"
