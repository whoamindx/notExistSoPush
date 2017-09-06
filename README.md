# notExistSoPush
> :repeat_one: Function that pushes a value in an array if it does not exist in the array
## Arguments
The first argument is the array, the second is the value to be pushed
```javascript
const ARR = [5,8,3,6];
notExistSoPush(ARR,6);
console.log(ARR);
// [5,8,3,6]
```
```javascript
const ARR = [5,8,3,6];
notExistSoPush(ARR,"Hello");
console.log(ARR);
// [5,8,3,6,"Hello"]
```
## Code
### ES5
```javascript
var notExistSoPush = function(arr,v){
	if(!arr.some(function(e){ return e == v })) arr.push(v)
};
```
### ES6 + ES7
```javascript
let notExistSoPush = (arr,v) => {
	if(!arr.includes(v)) arr.push(v);
};
 ```
