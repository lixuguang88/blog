#input type=text 的value值成了property
```html
<div  id="stateCate" style="display:none">
    <div class="state-cate">
        <div class="state-cate-group">
            <span class="btn"><button class="btn-inner">更改</button></span>
            <input type="text" value="游玩" name="cate" >
        </div>
    </div>
</div>
```
```javascript
var modal = null,
    html = $("#stateCate").html();
modal = APP.dialog(html, null, 236);
$(".state-cate input").val("赋新值无效"); //
```

解决办法

```html
<script  id="stateCate" type="text/tpl">
    <div class="state-cate">
        <div class="state-cate-group">
            <span class="btn"><button class="btn-inner">更改</button></span>
            <input type="text" value="游玩" name="cate" >
        </div>
    </div>
</script>
```
