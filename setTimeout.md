setTimeout是定時插入執行棧之後立即執行的

比如：

``` javascript
setTimeout(function(){while(1){}},6000);
setTimeout(function(){consolo.log(1)},10000);
setTimeout(function(){consolo.log(2)},4000);
```
會打印 2 然後進入循環 第二個setTimeout不會執行
