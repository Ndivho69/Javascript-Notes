
# Works from the back of the array 

# Pop function

> The pop function takes out the last element in the array, <br>
> assigning a variable to array.pop(), shows us that popped out element 


# Push function

> the push function adds a new element at the end of the array <br>
> assigning a variable to array.push, gives the length of the new array 


# Works from the front of the array

# THe shift function

> with the shift function you remove the first element in an array, <br>
> asssigning a varibale to the array.shift() will return the element which was removed in the array


# The unshift function

> the unshift function will add a new element at the front of the array <br>
> assigning a variable to the array.unshift will give you the length of the new array; <br>


`WHILE LOOP  while(condition){ final-expression }`

 # DOM Manipulation and Events

# Objects 
To create an bject, the object needs to have a `Key : Value`
* Where key is a string, and value can be anything.
* We can imagine an object as a cabinet with signed files. Every piece of data is stored in its file by the key. 
* It’s easy to find a file by its name or add/remove a file.
* to access an object the key is the indicator of where to look at exapmle if the object is
* `user = {name : "Ndivho"}`
* to access that i would have to `user[name]`;
or `user.name`



* In objects if the keys are listed in integers, they move in ascending order, visa-versa for strings

# Summary

* Objects are associative arrays with several special features.
* They store properties (key-value pairs), where:
   * Property keys must be strings or symbols (usually strings).
   * Values can be of any type.
* To access a property, we can use:
   * The dot notation: obj.property.
   * Square brackets notation obj["property"]. Square brackets allow taking the key from a variable, like obj[varWithKey].
* Additional operators:
   * To delete a property: delete obj.prop.
   * To check if a property with the given key exists: "key" in obj.
   * To iterate over an object: for (let key in obj) loop.
* What we’ve studied in this chapter is called a “plain object”, or just Object.
* There are many other kinds of objects in JavaScript:
   * Array to store ordered data collections,
   * Date to store the information about the date and time,
   * Error to store the information about an error.
   * …And so on.
* They have their special features that we’ll study later. 
* Sometimes people say something like “Array type” or “Date type”,
*  but formally they are not types of their own, but belong to a single “object” data type. 
*  And they extend it in various ways.
* Objects in JavaScript are very powerful.  
* Here we’ve just scratched the surface of a topic that is really huge. 
* We’ll be closely working with objects and learning more about them in further parts of the tutorial.

## Returning own keys in an object

> To return your own keys we use `Object.keys(objectName)` , this
> Will return keys that only belong to the object, excluding Inherited ones
>
## To Loop Over both inherited and own keys

> We can simply use the `the for loop`  and loop over our
> object, doing this will allow us to see all Keys, Inherited or not
> BUt if thats not what we want
 ## Built in method of finding Own keys in an object
>  That method would be `obj.hasOwnProperty(key)` 
> `for(let prop in rabbit) {
  let isOwn = rabbit.hasOwnProperty(prop);

  if (isOwn) {
    alert(`Our: ${prop}`); // Our: jumps
  } else {
    alert(`Inherited: ${prop}`); // Inherited: eats
  }
}`
# Javascript Prototypes
* Prototype attributes of object created with `new Object()`  or using the `Object Literal` ....
* All of them inherit from onject.prototype
* therefore Obj prototype is the prototype attribute of all objectts created with
* Meaning you can create any Object, without mentioning its properties, then use the `Object.prototype."name"` to add characteristics to that Object ,
* this is called `Prototype attributes`

## When an object is created with `var newObj = {} // Object Literals`;
* If an object is created like this, in order to add new properties into it we use `Object.prototype. "name"`
# When an object is created from a constructor function 
* We use the constructor to create new properties

 # Inheritance