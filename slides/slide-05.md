# Directives

Custom HTML attributes, elements, classes, or comments.

Some provided by Angular; can also create your own.


## Angular Provided Directives

Base functionality already available.

**Examples** - ng-app, ng-controller, ng-repeat, ng-click


## First Directive

    <div ng-app="MyApp"></div>

Declares the active area of our application.


## Creating your own Directives

    <button my-directive>Click!</button>
----
    app.directive('myDirective', function() {

      return function (scope, element, attrs) {
        element.bind('click', function() { alert('click!') });
      };

    });

Notice the camelcase to hypenated name conversion
