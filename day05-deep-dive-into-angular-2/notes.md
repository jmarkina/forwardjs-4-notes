# Deep Dive into Angular 2
Speaker : Aysegul Yonet [slide](http://yonet.github.io/ForwardJS-Angular2/#/)

* Pipes is the new term for filters

#### What's better
* Web workers are put to use and v
* Angular 2 is written in ES6
* Angular 1 was very slow for data binding
* NO MORE 2 way data biding in Angular2 but we can still do it and it's faster



#### TypeScript
TypeScript is a superset of JavaScript which primarily provides optional static typing, classes and interfaces. One of the big benefits is to enable IDEs to provide a richer environment for spotting common errors as you type the code.
For a large JavaScript project, adopting TypeScript might result in more robust software, while still being deployable where a regular JavaScript application would run.

```
class Greeter {
    greeting: string;
    constructor (message: string) {
        this.greeting = message;
    }
    greet() {
        return "Hello, " + this.greeting;
    }
}  
```

will result in 

```
var Greeter = (function () {
    function Greeter(message) {
        this.greeting = message;
    }
    Greeter.prototype.greet = function () {
        return "Hello, " + this.greeting;
    };
    return Greeter;
})();
```


#### Some new features for Angular 2
* `()` are for events
* `[]` are for attributes
* `*` is for changing the dom
* `ng-for` is for repeating (`ng-repeat` previously)
* `ng-if` condition etc...
* Data flows into a directive via property bindings.
* Data flows out of a directive via event bindings.
* You can use property and event bindings to implement two-way bindings.
* Angular provides syntax sugar for two-way bindings, interpolation, and passing constants.
* Module syntax
``` JavaScript
//lib.js
export function square(x) {
 return x * x;
}
// main.js
import { square } from 'lib';
```

* When we assign styles to a component they are scoped to that specific component. Our styles will only apply to our AppComponent and won't "leak" to the outer HTML.









