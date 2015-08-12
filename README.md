#
   
##[手机软键盘遮挡输入框](./scrollIntoView.md)
```html
<input type="text" value="" id="content" name="content">
```
```javascript
document.querySelector("#content").addEventListener("focus", function(){
       var that = this;
       //等待软键盘弹出
       setTimeout(function(){
           that.scrollIntoView();
       }, 200);                   
}, false);
```
