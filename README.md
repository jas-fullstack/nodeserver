#### sudo npm init
#### touch index.js

```` 
const express = require('express');
var bodyParser = require("body-parser");
const app = express();
app.use(bodyParser());
app.get('/',(req,res)=>{
    console.log("hi");
    res.send("basic app working")
});

app.listen(3000,()=>{
    console.log("app is working on poer 3000");
}); 
````
### sort number with loop 
````

function sortArray(array) {
  var temp = 0;
  for (var i = 0; i < array.length; i++) {
    for (var j = i; j < array.length; j++) {
      if (array[j] < array[i]) {
        temp = array[j];
        array[j] = array[i];
        array[i] = temp;
      }
    }
  }
  return array;
}

console.log(sortArray([3,1,2]));
````


````

// Question:
// Have the function FindIntersection(strArr) read the array of strings stored in strArr which will contain 2 elements: the first element will represent a list of comma-separated numbers sorted in ascending order, the second element will represent a second list of comma-separated numbers (also sorted). Your goal is to return a comma-separated string containing the numbers that occur in elements of strArr in sorted order. If there is no intersection, return the string false.


// Input: ["1, 3, 4, 7, 13, 15", "1, 2, 4, 13, 15"]
// Output: 1,4,13

function strArr(arr){
        //console.log(arr[0],"---" ,arr[1]);
        console.log("===",arr[0].split(","))
        const data1 = arr[0].split(",");
        const data2 = arr[1].split(",");
        var matched = [];
        data1.map((val)=>{
            data2.map((val2)=>{
                
                    if(val == val2){
                        matched.push(val)
                    }
            })
        })
        console.log(matched)
    
}
console.log(strArr(["1, 3, 4, 7, 13, 15", "1, 2, 4, 13, 15"]))
````

````
###reverse number
function reverseString(str) {
    var newString = "";

    for (var i = str.length - 1; i >= 0; i--) { 
    	console.log(i)
        newString += str[i]; // or newString = newString + str[i];
    }
    return newString; // "olleh"
}
 
console.log(reverseString('hello'));
````
