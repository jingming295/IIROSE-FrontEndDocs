# Utils.uploadImg()

```javascript
Utils.uploadImg(e, t)
```

```e```: 文件对象
```t```: 回调函数，接收一个xhr对象

### 上传

- 使用例子

```javascript
// 创建一个模拟的 File 对象
const file = new File(['This is a mock file content'], 'mockfile.txt', { type: 'text/plain' });

// 调用 Utils.uploadImg()，传入模拟的文件对象和处理响应的回调函数
Utils.uploadImg(file, function(xhr) {
  if (xhr.readyState === 4) {
    if (xhr.status === 200) {
      // 处理上传成功的逻辑
      console.log('File uploaded successfully!');
      console.log(xhr.responseText); // 响应内容
    } else {
      // 处理上传失败的逻辑
      console.error('Upload failed. Status:', xhr.status);
    }
  }
});
```

在回调的函数中，你将会得到xhr对象。xhr下的responseText就是文件路径，你需要和```http://r.iirose.com/```进行拼接

- 效果：

![上传成功](https://static.codemao.cn/i/24/4/17/16/4935-IZ.png)
