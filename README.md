<img src="https://devmounta.in/img/logowhiteblue.png" width="250" align="right">

# Project Summary

In this project, we'll create an Angular application that displays a list of your friends. The list will be searchable and filterable through user interaction. You can see a live demo by clicking on the link below.

Live example: <a href="https://devlemire.github.io/angular-1-afternoon/">Click Me!</a>

## Setup

* Fork and clone this repository.
* Open the project directory in your coding IDE.

## Step 1

In this step, we'll create the skeleton of our Angular application.

### Summary

* Create a `js` folder at the root of the project.
* Create an `app.js` file in `js/`.
* Create a `friendCtrl.js` file in `js/`.
* Open `js/app.js` and create a new Angular application called `"myApp"`.
* Open `js/friendCtrl.js` and create a controller called `friendCtrl`.
  * Add a scope variable called test that equals `"Connected"`.
* Open `index.html`.
* Add a `script` tag for the Angular CDN.
* Add a `script` tag for `js/app.js`.
* Add a `script` tag for `js/friendCtrl.js`.
* Add `ng-app` and `ng-controller` to the HTML.
* Verify your `app` and `controller` are connected by adding `{{ test }}` to the HTML.
  * If `Connected` appears on the DOM, remove `{{ test }}` from the HTML and `$scope.test` from `js/friendCtrl.js`.

<details>

<summary> Detailed Instructions </summary>

<br />



</details>

### Solution

<details>

<summary> <code> index.html </code> </summary>

```html
<!DOCTYPE html>
<html ng-app="myApp">
  <head>
    <title>Angular Friends</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css">
    <link rel="stylesheet" type="text/css" href="styles.css">
  </head>

  <body ng-controller="friendCtrl">
    <h1>The <strong>facebook</strong> Friend Machine</h1>

    <div class="friends">
      <form class="form-inline searchForm" role="form">
        <div class="form-group">
          <input class="form-control" placeholder="Search Anything About Your Friends">

          <select class="input-medium">
            <option>Name</option>
            <option>#Friends</option>
            <option>City</option>
            <option>State</option>
            <option>Country</option>
          </select>

          <select class="input-medium">
            <option value="-">Descending</option>
            <option value="+">Ascending</option>
          </select>
        </div>
      </form>

      <ul>
        <li class='friend'>
          <img class="profile-pic" src='http://placebear.com/50/50.jpg'>
          <h3>Cali Fornia</h3>
          <div class="location">
            Location: New Port Beach, California, United States
          </div>
          <div class="status">
            Status: I hate the snow. I wish I was on the beach right now!!!
          </div>
          <div class="num-friends">
            Friends: 1,367
          </div>
        </li>
      </ul>
    </div>

    <script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <!-- your scripts here -->
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.6/angular.min.js"></script>
    <script src="js/app.js"></script>
    <script src="js/friendCtrl.js"></script>
  </body>
</html>
```

</details>

<details>

<summary> <code> js/app.js </code> </summary>

```js
angular.module("myApp", []);
```

</details>

<details>

<summary> <code> js/friendCtrl.js </code> </summary>

```js
angular.module("myApp").controller("friendCtrl", function( $scope ) {
  
});
```

</details>
