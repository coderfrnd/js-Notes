# JS BASIC NOTES

### What is  Mutable and Immutable Methods (in strings and arrays) ?
so before moving to solve this question first we need to understand what is 

**Mutable and Immutable datatypes** 
--
**Mutable Datatypes (Non-Primitive)** In simple word mutable can be changed without creating a new reference There are only three datatypes are mutable in js 
like 
```js
function(){

}
let arr = []
let obj ={

}
// This things are mutable 
```

**Immutable Datatypes (Primitive Data Types)** In simple word immutable can not be changed without creating a new reference They are stored directly in memory
```js
let num =10  // Immutable
let str = "HELLO" //Immutable
Booleans (Boolean) //Immutable
Null (null) //Immutable
Undefined (undefined) //Immutable
// Basically it does not modify like if we want to do 
str[0] == "A" // Not changing because string is immutable 
// but one question is that we can change 
num = 11
str = "WORLD"
// here it changes so how this are immutable here we are not modifiying it we replace it like in immutable we cant modify it but we can completely replace it  
Immutable data types cannot be changed once they are created. If modified, a new value is created instead.
```

so ans of the question is String is IMMUTABLE AND ARRAY IS MUTABLE 

### Pass by Reference and Pass by Value 

**Pass by value -**
In a pass by value if we modify or do something so original datatypes remain unchanges but pass by reference if i do something then original datatypes changed
```js
// Example based on pass by value 
let n =5;
function x(n){
  n++;
  console.log(n)
}
console.log(n) // before call fn 5 op 
x(n) // inside fn print 6 op
console.log(n) // here again print 5
// so this means global n not updated outside fn but inside it updated so here the actual value of n is not changed
```
**Pass by Refernece -** Here if we pass datatype and do some changes then original value/datatype will be changed eg -: Array,Object,function

```js

let obj = {
  name:"unknown",
  age:00
}
console.log(obj)

function filldetails(obj){
  obj.name = "Abhishek"
  obj.age = 23
  console.log(obj)
}
filldetails(obj) // Here obj value changed and it changed everywhere after that
console.log(obj) // Here also changed 
```






