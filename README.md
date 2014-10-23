angular-quill
================

Angular Quill is an angular directive for the Quill editor.  http://quilljs.com/


Usage
--------------

1. Include the quill libraries
2. In your angular application register angular-quill as a dependency.
3. Add the necessary html to view the editor.

Registration

```js

// Angular Registration
angular.module('app', ['angular-quill']);

```

Bare Minimum Html
```html
<div ng-model="article" quill></div>
```

With Options
```html
 <div ng-model="article" quill="{
      modules: {
        'toolbar': { container: '.toolbar' },
        'image-tooltip': false,
        'link-tooltip': false
      },
      theme: 'snow'
    }"></div>
```

You can pass options directly to Quill editor by specifying them as the value of the `quill` attribute.


Bower Installation
--------------
```js
bower install angular-quill
```
