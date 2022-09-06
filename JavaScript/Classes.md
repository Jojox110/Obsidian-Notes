Getters and Setters:

Getter: GET said value, no modifying in anyway
Setter: SET said value, goal of modifying/assigning

Syntax:

get methodName(): // takes no arguments
	return value

set methodName(value): // takes one argument
	// logic, assigning or modifying something related to the input or context of usage

There's other ways to make "smarter get/set", look up when needed


Strict Mode:

- Stricter Syntax
- Better performance
- Silent errors can be thrown


Static keyword:

- Can be called without instantiating their class
- Cannot be called through a class instance


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

- Does not require let, const or var before declaring the variable name. You can put # in front of the name to make it a private field

```
class User {
	name = "John"
}
```

The name variable is a class field, which you can only use in the class. It does not put it into the class prototype and you can use more complex expressions in the class field like a prompt for example 



Pros and Cons of using classes:

Pros:

- Easier syntax if you are used to OOP
- An extra options for object creation


Cons:

- Bad for functional progrtamming - but classes can be ignored if that's the goal
- Not the same as other languages like Java, which uses classes a lot more


