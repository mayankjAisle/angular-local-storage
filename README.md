angular-local-storage
=====================

An Angular module that gives you access to the browsers local storage

Remember to set your app name (settings.appPrefix) in the settings at the beginning of localStorageModule.js.

To do:
- Set cookies as a failback for browsers that do not support local storage
- Expand Readme

Example use: 

```javascript
angular.module('yourModule', ['LocalStorageModule'])
.controller('yourCtrl', [
  '$scope',
  'localStorageService',
  function($scope, localStorageService) {
    // Start fresh
    localStorageService.clearAll();
    localStorageService.add('Favorite Sport','value');
}]);
```
