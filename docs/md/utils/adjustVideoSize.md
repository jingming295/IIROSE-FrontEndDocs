# adjustVideoSize

## Utils.adjustVideoSize(e,t,o,i,a,s)

> 设置聊天室视频大小

```javascript
Utils.adjustVideoSize(e,t,o,i,a,s)
```

```e```: 要调整大小的视频元素，通常是一个 jQuery 对象或者 DOM 元素

```t```: 视频的宽高比，通常是一个包含两个数字的数组，例如 [16, 9] 表示 16:9 的宽高比。

```o```: 一个布尔值，表示是否应该使用动画来调整大小。

```i```: 视频的原始宽度和高度，通常是一个包含两个数字的数组，例如 [1920, 1080]

```a```: 一个布尔值，表示是否要在视频调整大小后底部对齐。

```s```: 一个数字，表示视频容器的高度，用于计算调整后的视频大小。(未经验证)

### 设置聊天室视频大小

- 使用例子

```javascript
let video = document.getElementById('videoPlayer')
let jQueryVideo = $(video);
Utils.adjustVideoSize(jQueryVideo, null, 1, [1920, 1080], 1, null);
```

- 效果：

![设置聊天室视频大小](https://static.codemao.cn/i/24/4/29/11/1243-EV.png)

---