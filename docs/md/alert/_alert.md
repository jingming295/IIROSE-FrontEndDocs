# 消息

## 弹出消息

> 弹出消息

### 函数

```javascript
_alert(e, t, o, i, a) 
```

```e```: 需要被显示的消息。

```t```: 这是一个数组，为真的话将会更改消息的呈现方式，我不确定还有没有别的用途。

```o```: 这是个布尔值，表示是否要对 e 的内容进行 HTML 转义。

```i```: 这是一个可选的字符串，我不确定这个能干什么。

```a```: 我不确定这个是不是和页面失焦这些有关

```javascript
var config = [
  "提示框标题",
  "这是提示框的内容",
  "http://r.iirose.com/i/21/10/19/20/1347-OZ.jpg#e"
];
_alert("&lt;消息&gt;", config, true, '测试', true);
_alert("&lt;消息&gt;", null, true, '测试', true);
_alert("&lt;消息&gt;", null, false, '测试', true);
```

- 效果：

![_alert](https://static.codemao.cn/i/24/4/17/23/0907-NX.png)