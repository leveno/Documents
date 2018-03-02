## 编写此文档的意义是为了熟悉整个项目开发过程

$ mkdir myapp  
$ cd myapp  
$ npm init  
$ npm install express --save  
$ npm install express  
$ touch app.js  
```
  var express = require('express');
  var app = express();

  app.get('/', function (req, res) {
    res.send('Hello World!');
  });

  var server = app.listen(3000, function () {
    var host = server.address().address;
    var port = server.address().port;

    console.log('Example app listening at http://%s:%s', host, port);
  });
```

$ node app.js  
http://localhost:3000/ 

## Express生成器
$ npm install express-generator -g  
$ express -h  
$ express myapp  
$ cd myapp   
$ npm install   
linux: $ DEBUG=myapp npm start    
window: > set DEBUG=myapp & npm start  
http://localhost:3000/ 
