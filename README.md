#sudo npm init
#touch inde.js

const express = require('express');
const app = express();

app.get('/',(req,res)=>{
    console.log("hi");
    res.send("basic app working")
});

app.listen(3000,()=>{
    console.log("app is working on poer 3000");
});
