# JavaScript Syntax Notes

## 01. Values, Types and Operators

```js
let variableName // Declare variable
const variableName // Declare constant
console.log(stuff) // Print to console
```

## 02. Program Structure

### If else

```js
if (condition){
	// Stuff
}
else if (condition){
	// Stuff
}
else{
	// Stuff
}
```

### Loops

```js
for (let i=0; i<=10; i+=1){
	// Stuff
}

while (condition){
	// Stuff
}

do {
	// Stuff
}
while (condition);
```

## 03. Functions

```js
let functionName=function(parameters){
	// Stuff
};

function functionName(parameters){
	// Stuff
};

let functionName = (parameters) => {
	// Stuff
};

// If you write "...paramters", function will store all paramters inside the parameters list
```

## 04. Data Structures

### Array = List

```js
let listName=[element1, element2...] // Make a list
let listName=[e1,...anotherList,e2] // Add anotherList in listName
listName[id] // Element of list at id
listName.length // Total elements
listName.push(element) // Add element to end and return new list length
listName.unshift(element) // Add element to front
listName.pop() // Delete last element and return it
listName.shift() // Delete first element
listName.includes(element) // true if element in list
listName.indexOf(element) // 1st location from left where element is found, -1 if not found
listName.lastIndexOf(element) // From right
listName.slice(fromId,untilId) // List from fromId(included) to untilId(not included, default until end)
listName.concat(anotherListOrElement) // Add list to list
```

### Object = Dictionary

```js
let objName={"key1":value1, "key2":value2...} // Make an object
objName["key1"] // Element of object
objName.key1 // Also works when key is named as a variable
delete objName.key1 // Delete an element
"key1" in ObjName // true if key1 exists
Object.keys(ObjName) // List of keys
Object.assign(Obj1, Obj2) // Merge Obj2 into Obj1
```

### Strings

```js
string.length // Total characters
string[id] // Char of string at id
string.slice(fromId,untilId) // Substring from fromId(included) to untilId(not included, default until end)
string.indexOf(substring) // 1st location from left where substring is found, -1 if not found
string.lastIndexOf(substring) // From right
string.padStart(maxLength,padChar) // Add padChars at front until string is of maxLength
list = string.split("{at}") // split string
string = list.join("{with}") // join list element to string
```

### Loop through Array or String

```js
for (let element of list){
	// loop through all elements
}

for (let id in list){
	// loop through ids of elements
}
```

### Math object

```js
Math.property();
//min, max, abs, round, floor, ceil, cos, sin etc
```

### JSON

```js
jsonString = JSON.stringify(object) // convert object to json
object = JSON.parse(jsonString) // convert json to object