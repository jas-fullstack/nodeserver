#sudo npm init
#touch index.js

```` const express = require('express');
var bodyParser = require("body-parser");
const app = express();
app.use(bodyParser())
app.get('/',(req,res)=>{
    console.log("hi");
    res.send("basic app working")
});

app.listen(3000,()=>{
    console.log("app is working on poer 3000");
}); ````
