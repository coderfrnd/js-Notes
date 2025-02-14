# JS BASIC NOTES ON ARRAY
### Array 
Array is a Data structure which can store multiple variables in a single variable and access them using index value baiscally it is order collection where we can store variable in a groups

**How to declare and use array ?**

```JS
// How to declare array 
let x = [] // here this is a method of declaring it is resizable

x.push(5) // this is a method of push value in array and every time when we push value it append from back

x.pop() // Every time when use array.pop it removes element from back it does not take any element
```

#### Array.concat
```JS
// In this method basically we combine two array into single array 
let arr1 = [1, 2, 3];
let arr2 = [4, 5, 6];
let arr3 = [7, 8, 9];

let result = arr1.concat(arr2,arr3);

console.log(result); // [1, 2, 3, 4, 5, 6, 7, 8, 9]
console.log(arr1);   // [1, 2, 3] (original array remains unchanged)
console.log(arr2); 
```
#### Array.slice
```JS
// .slice(startIndex,endIndex) but endIndex is excluded 

let arr1 = [1, 2, 3, 4, 5, 6];

console.log(arr1.slice(0,3))

Output:

[ 1, 2, 3 ]
```
#### Array.splice
```JS
// syntax
let arr1 = [1, 2, 3, 4, 5, 6];


console.log(arr1.splice(1,3,66)) // here it removed 2 3 4 and add 66 in place of this three 
splice takes three argument first is start index from where starting happen and second one is how many index need to be removed and last one is what u want to add 
It removes the element without leaving gaps.
The array remains continuous.
console.log(arr1) // op us 

Output:

[ 2, 3, 4 ] // its showing what is going to be removed
[ 1, 66, 5, 6 ]
// 
```
#### Array.join()
```JS
// syntax arr.join() here inside join method it takes argument of paramerter like seprator what i want to add in the middle by default it was , 
let arr = ["abhishek", "jaiswal", "mzp"]

console.log(arr.join())
console.log(arr.join("-"))
console.log(arr.join("|"))
Output:

abhishek,jaiswal,mzp
abhishek-jaiswal-mzp
abhishek|jaiswal|mzp
```

### Finding method
 #### find method
```JS
// syntax is arr.find(fn,thisvalue)

let arr = ["abhishek", "jaiswal", "mzp"]
let k = arr.find((ele)=> ele == "abhishek")
let r = arr.find((ele)=> ele == "abhishe")
console.log(k)
console.log(r)

// only single value will be find by this method and the first value which arrive  and it takes two argument one is fn and onetherone is this value inside fn it can takes 3 arguments 2 are optional those 3 parameter are current value ,index,array if it not able to find value then it returns undefined

Output: 
abhishek
undefined
```
#### Array.indexof

```JS
// syntax-->
// indexOf(searchElement)
// indexOf(searchElement, fromIndex)
// it return the index of array in which element is present  it any thing is not found it returns -1 it uses === for strictly checking element is present or not 

let arr = [1, 2026 , 5 ,6,8,9]

console.log(arr.indexOf(5))
console.log(arr.indexOf(5,4))

Output:
2
-1

```
#### Array.includes
```js
// includes(searchElement)
// includes(searchElement, fromIndex)
//  this is the syntax of includs it basically return true and false it means value is present or not  from index and fromIndex is inclusive means search from that index to the end it uses === for checking 
let arr = [1, 2026 , 5 ,6,8,9]


console.log(arr.includes(2020))
console.log(arr.includes(6))

Output:

false
true

```
#### Array.findIndex
```js
// syntax
array.findIndex(function(currentValue, index, arr), thisValue)
// This property is different from indexof and it work on object else indexof not work on object and it take callback fn it work on most complex cases  when searching with a condition 
let arr = [1, 2026 , 5 ,6,8,9]

let p = arr.findIndex((ele) => ele==2026)
console.log(p)

Output:

false
true
1


```