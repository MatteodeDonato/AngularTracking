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
myapp = angular.module('myapp', ["ui.router"]);
myapp.config(function($stateProvider, $urlRouterProvider){
$urlRouterProvider.otherwise("/default")

$stateProvider
 .state('option', {
  url : "/url",
  templateUrl : "url.html"
  controller : function($scope){
   //declarations
   //$scope.variable = ...
   }
   })
   
   })

