# createJsPlayer

## Utils.createJsPlayer(e,t,o,i)

> 创建一个视频播放器（我不确定）

```javascript
Utils.createJsPlayer(e,t,o,i)
```

```e```: 数字，如果为0就尝试使用 HLS 播放器，其他则尝试使用 FLV 播放器

```t```: 用于存储创建的视频播放器对象，包括 HLS 播放器和 FLV 播放器。

```o```: 视频的链接或源文件地址

```i```: 回调函数，用于处理播放器创建失败时的情况

### 创建一个视频播放器（我不确定）

- 使用例子

```javascript
// 创建一个包含 HLS 播放器的对象
let y = {
    hls: new Hls() // 创建一个新的 HLS 播放器对象
};

let o = 'https://r.iirose.com/m/24/3/25/11/2245-ZE.mp4'

function i(res) {
    console.log(res);
}

Utils.createJsPlayer(0, y, o, i);
```

- 以上代码执行了不会报错，但是我也没看出来发生了什么。

- 效果：

![判断](https://static.codemao.cn/i/24/4/30/19/2745-XY.png)

---