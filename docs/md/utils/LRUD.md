# LRUD

## Utils.LRUD(e)

> 打开或关闭小聊天框(暂时叫这个名字)

```javascript
Utils.LRUD(e)
```

```e```: 包含一个preventDefault的回调函数。可以不需要传入这个参数


### 打开或关闭小聊天框

- 使用例子

```javascript
// 如果你想传入参数 e，并调用 e.preventDefault()，可以这样做：
var fakeEvent = {
    preventDefault: function() {
        console.log("Prevent default action called!");
    }
};
Utils.LRUD(fakeEvent);
```

- 效果：

![小聊天框](http://r.iirose.com/i/24/4/28/21/3659-K2.png)

---