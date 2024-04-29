# blobToDataURL

## Utils.blobToDataURL(e,t)

> 将 Blob 对象转换为 Data URL

```javascript
Utils.blobToDataURL(e,t)
```

```e```: Blob对象

```t```: 回调函数

### 将 Blob 对象转换为 Data URL

- 使用例子

```javascript
// 创建一个示例的 Blob 对象，可以是任何数据，比如一个字符串或者一个 ArrayBuffer
var myBlob = new Blob(["Hello, world!"], { type: "text/plain" });

// 调用 blobToDataURL 函数，并传入这个示例的 Blob 对象
Utils.blobToDataURL(myBlob, function(dataURL) {
    // 在这里处理转换后的 Data URL
    console.log(dataURL);
});
```

- 效果：

![转换](https://static.codemao.cn/i/24/4/29/12/1652-XW.png)

![转换](https://static.codemao.cn/i/24/4/29/12/1733-PK.png)

---