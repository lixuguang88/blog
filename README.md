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
   
   
## [git bash pull/push配置无密码提交/同步]
git bash(terminal) 上pull/push的时候每次提交都会显示 Enter passphrase for key '/c/Users/xxx/.ssh/id_rsa':  
1.xxx    
2.yyy  
