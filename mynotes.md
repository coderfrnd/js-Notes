# JS BASIC NOTES

## Loops --->

There are many iterative methods in JavaScript for iterating over an array, string, or object.

### **For Loop**
The `for` loop allows you to run code multiple times.here the syntax of for loop

```js
for (let i = 0; i < array.length; i++) { 
    // Some code stuff
}
```
### **forEach loop**
This loop work on only array It take one callback fn and this value so this value is refferd to a like if you pass a object and want to perform action then you can use this value else that is optional

```js
array.forEach(function(currentValue, index, arr), thisValue){
          
}
```
Here function is callback function and thisvalue is optional 

### **for in loop**
This loop is used for object mainly we can use this on array but it is not recommended it iterate over keys in array it considered array index as a key so thats why it work on array and else everything in the top of end is object in JS

```js
for(let key in objectname){
    // if want to access key the just write
    console.log(key)
    // if want to access value then write objectname[key]
    console.log(objectname[key])
}
```
### **for of  loop**
This loop is work on arrays, strings, maps, sets it is designed for iterate on iterable object it is not work on Objects bcz they are not iterable by default because they dont have any ordered keys like array or string where index worked as ordered string

```js
for(let num of arrayname){
    // in a place of array name we can write set name and map name also 
    console.log(num)
    // array value in index by appears
}
```
### **while loop**
This loop is worked on a condition which is provide as a argument if that condition is failed or false then loop break

```js
while(condition){
// any condition like iterate until 20 not become zero etc etc
}
```