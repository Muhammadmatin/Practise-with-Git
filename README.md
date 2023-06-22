
# `Lecture-4`
## TABLE OF CONTENTS
```sh
1 - ARRAY
2 - ARRAY METHODS
3 - DESTRUCTRING
4 - SPREAD & REST
```

#  What is `Array` in `Javascript`?
> An array is an object that holds values (of any type) not particularly in named properties/keys,but rather in numerically indexed position In JavaScript, an array is an ordered list of values. Each value is called an element specified by an index.First, an array can hold values of mixed types. An array is a special variable, which can hold more than one value:

#### Creating an `Array`
```sh
Using an array literal
const array=[1,2,3,4,5]
log - array => [1,2,3,4,5]
```
## Change elements in `array`
- You can also add elements or change the elements by accessing the index value
Suppose, an array has two elements. If you try to add an element at index 3 (fourth
element), the third element will be undefined. For example,

```sh
#example
let arr = ["go","sleep",1,2,true]
arr[3]=2
log arr === => ["go","sleep",2,2,true]
```

# `Array` methods
|POP|`FOREACH`|JOIN|
|-----|-----|-----|
|SHIFT|`MAP`|INCLUDES|
|PUSH|`FIND` |INDEXOF|
|UNSHIFT|`FILTER` |SPLICE|
|CONCAT|`REDUCE` |TOSTRING|
|SLICE|`toSorted` |TOREVERSED|

##### `Array` method `push`
- This method add a new element from the end of the arr and return new length of arr
```sh
let arr = ["banana","kivi","apple"]
arr.push("orange")
log arr === => ["banana","kivi","apple","orange"]
```
##### `Array` method `pop`
- This metod removes one element from the end of the arr
```sh
let arr = [1,2,3,4,5]
log(arr.pop()) === => [1,2,3,4]
```
##### `Array` method `unshift`
- This method adds more one elements from the start of the arr
```sh
let arr = [2,3,4,5]
log(arr.unshift(0,1)) === [0,1,2,3,4,5]
```

##### `Array` method `shift`
- This method removes the element from the start of the arr
```sh
let arr = [0,1,2,3]
log (arr.shift()) === => [1,2,3]
```
##### `Array` method `toString()`
- This method retunrs arr to the string
```sh
let arr = [1,2,3,4]
log (arr.toString()) === 1,2,3,4
```
##### `Array` method `indexof()`
- This method show the position of the elements if it can`t find returns -1.

##### `Array` method `includes`
- This method work like searching it will return only true and false.

##### `Array` method `slice`
- This method mean start from the n index till n index.

##### `Array` method `concat`
- This method add an arrays with each other.

##### `Array` method `splice`
- This method includes 3 values `(1)from which index` + `(2)-How many elements add to arr`   +  `(3)-the values of element`
 
# JAVASCRIPT ARRAY METHOD `CALLBACKS`
## `1 - MAP`
- This method create a new arr and it has a callbacks which takes 3 items.
```sh

// let nums =[4,4,5,6,7,8]
// let s = 0
// let nums1 = nums.map(function(item,index,arr) {
//     return index+item%2==0
// })
// console.log(nums1);
```
## `2 - FOREACH`
- THIS METHOD WORKS LIKE A LOOP ITS MORE COMFORTABLE
```sh
const numbers = [1, 2, 3, 4]

numbers.forEach((num) => {
  const square = num * num
  console.log('Квадрат числа равен: ' + square)
})

```
# `3 - FIND`
- THIS METHOD RETUND THE FIRST VALUE THAT IT FIND AND RETURN `UNDEFINED` IF IT DOESN`T FIND ANYTHING
```sh
function plan(item,index,arr){
    let myplan = "go to 102"
    return element===myplan
}
let plantomorrow = "go to balh","stay there",
console.log(plantomorrow.find(plan)
```
# `4 - REDUCE`
- The reduce() method executes a user-supplied "reducer" callback function on each elementof the array, in order, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value 
```sh
let s = [1,2,3,4]
let s1 = s.reduce(function(a, b) {
    return a+b
})
console.log(s1);
```
# `5 - FILTER`
- This metod creates a shadow copy of a portion given arr
```sh
let s1 = [1,2,3,4,5,6,7,8]
let s2 = s1.filter(n=> n<5)
console.log(s2);
```
# `6 - TOSORTED`
- The sorted method of arr is copying version of the sort () method. it returns a new arr with elements sorted in ascending order.
```sh
// let a = [234,3,465,234,5,6]
// let b = a.toSorted((a,b) => a-b)
// console.log( b);
```
# `METHOD DETSRUCTURING`
- WE USE THIS METHOD TO MAKE A VARIABLES FROM THE ARR OR OBJECTS
```SH
 let arr = [1,2,3]
 let [a,b,c] = [...arr]
 console.log(a+b+c);
```

# `REST`
- WE USE THIS METHOD TO MAKE STRINGS OR NUMBERS INTO ARR
```SH
function sum(...sum) {
return sum
}
console.log(sum(1,2,3,4,5));
```

# `SPREAD`
- The spread (...) syntax allows an iterable, such as an array or string, to be
expanded in places where zero or more arguments (for function calls) or
elements (for array literals) are expected. In an object literal, the spread syntax
enumerates the properties of an object and adds the key-value pairs to the object
being created.
```SH
let arr=[1,2,3]
let arr1=[...arr]
arr1.push("hi")
console.log(arr); == [1,2,3."HI"]
```
