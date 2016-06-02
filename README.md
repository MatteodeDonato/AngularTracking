# AngularTracking
A Basic single page app using AngularJS.

The app is designed primarily just as a a proof of concept for tracking in single page applications. It also serves the purpose of being a place to experiment with various web technologies.

### Goals

- JSON
  * what is it?
  * learn it!
- REST Service Calls
- tracking JSON service calls

- analytics
 * google
 * angulartics
 * segment
 * *which is the best?*
   * compare

### Basic format of a `script.js` file w/ Angular


```javascript
var myapp = angular.module('myapp', ["ui.router"])
myapp.config(function($stateProvider, $urlRouterProvider){

  // For any unmatched url, send to /route1
  $urlRouterProvider.otherwise("/page1")

  $stateProvider
    .state('page1', {
        url: "/page1",
        templateUrl: "page1.html"
    })
      .state('page1.list', {
          url: "/list",
          templateUrl: "page1.list.html",
          controller: function($scope){
          }
      })

    .state('page2', {
        url: "/page2",
        templateUrl: "page2.html",
        controller: function($scope){

        }

    })

```
