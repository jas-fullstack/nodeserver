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
