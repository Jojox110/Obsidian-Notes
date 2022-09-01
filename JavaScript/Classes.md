Getters and Setters:

Getter: GET said value, no modifying in anyway
Setter: SET said value, goal of modifying/assigning

Syntax:

get methodName(): // takes no arguments
	return value

set methodName(value): // takes one argument
	// logic, assigning or modifying something related to the input or context of usage

There's other ways to make "smarter get/set", look up when needed


Classes:

```
class User {
	constructor(name) {
		this.name = name
	}

	sayHi() {
		alert(this.name)
	}
}
```

Methods, such as sayHi, are put in the class prototype

Classes in JS are often know as Synactic Sugar, but there is still a few differences:

- Unique special internal property IsClassConstructor - you have to use the new property to create a new object using the class
- Class methods are non-enumerable
- Classes always use strict



Class Expressions:

```
let User = class {
	sayHi() {
		alert("Hello")
	}
}
```

It is also possible to make classes on-demand dynamically

```
function makeClass(arg){
	return class{
		// logic
	}
}
```

You can also put getters and setters in classes


Class Fields (newer feature, may not work on older browsers):

```
class User {
	name = "John"
}
```

The name variable is a class field, which you can only use in the class. It does not put it into the class prototype and you can use more complex expressions in the class field like a prompt for example 