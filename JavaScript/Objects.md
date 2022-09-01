Objects:

```
const myObject = {
	property: "Value!",
	otherProperty: 77,
	"obnoxious property": function(){
		do something
	}	
}
```


Ways to get information:
- myObject.property (can only be used for one word names, but cleaner and preferred)
- myObject[property] (multiple word names must be in quotes "")


Object Constructors:

```

function Player(name, marker) {
	this.name = name
	this.market = marker
}
```

const player = new Player("steve", "X")


Notes for classes: [[Classes]]