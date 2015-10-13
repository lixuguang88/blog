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
   
   
## [git bash(terminal)配置无密码提交/同步](./gitbashnopassphrase.md)
git bash(terminal) 上pull/push的时候每次提交都会显示 Enter passphrase for key '/c/Users/xxx/.ssh/id_rsa':  

## [parseInt("09")ie8(包括以前)返回0](./parseInt-ie8-error.md)
parseInt("09"), parseFloat("09"), Number("09")  
IE8的返回值 0, 9, 9

## [上面div层的touch事件 影响下面div层的click事件](移动端触发touch事件同时触发click事件的相关解决方法)

## window.innerWidth, window.innerHeight 得到屏幕的可用宽度和高度的问题(iOS)
在页面底部直接加如下代码, (得到宽度和告诉是document的!!!)
```javascript
alert(window.innerWidth + ":::" + window.innerHeight);
```
   
```javascript
window.onload = function(){
   alert(window.innerWidth + ":::" + window.innerHeight);
}
//or
$(document).ready(function(){
   alert(window.innerWidth + ":::" + window.innerHeight);
});
```

## [iOS里面对竖拍的图片展示位竖的，Android里面展示位横的](./EXIF.md)
iOS里面自动旋转图片，图片的长度和宽度没有一块更新。
   
[java](https://github.com/drewnoakes/metadata-extractor)后台读取图片exif的信息,后台旋转图片的方向.   
```html
[Exif] Orientation - Top, left side (Horizontal / normal) 
[Exif] Orientation - Right, top side (Rotate 90 cw) 
```
Orientation Rotate只保存默认的旋转，也就是用户自己保存旋转的是正常的（也就是Top, left side (Horizontal / normal)）。
   
   
## [如何解决failed to push some refs to git](http://jingyan.baidu.com/article/f3e34a12a25bc8f5ea65354a.html?st=2&net_type=&bd_page_type=1&os=0&rst=&word=chegji@gmail.com)
 ```javascript
 //先执行
 git  pull --rebase origin master
 //在执行push
 git push -u origin master





