```javascript
/* This function accepts two parameters: an array of arrays, and an empty 
array that will ultimately contain our averages. Each nested array is a 
collection of number values. */

function arrayAverages(arrArr, newArr) {
  for(var i = 0; i < arrArr.length; i ++) {
    newArr.push(arrArr[i].reduce(function(prev,cur){
      return (prev + cur)
    })/arrArr[i].length);
  }
}

array1 = [1,2,3,4,5];
array2 = [2,4,6,8,10];

dataArray = [array1, array2];
result = [];

arrayAverages(dataArray, result);  // [3,6]
```
