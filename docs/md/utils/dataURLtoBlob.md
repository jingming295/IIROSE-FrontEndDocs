# dataURLtoBlob

## Utils.dataURLtoBlob(e)

> 将 Data URL 转换为 Blob 对象

```javascript
Utils.dataURLtoBlob(e)
```

```e```: Data URL

### 将 Data URL 转换为 Blob 对象

- 使用例子

```javascript
const dataURL ="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAlgAAAJYAQAAAACWHaVxAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QAAd2KE6QAAAAHdElNRQfnCBQKEiERlO/IAAAAuElEQVR42u3MQREAAAQAMHf6d9KMEl5sARbBCdlbyuVyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuVwul8vlcrlcLpfL5XK5XC6Xy+VyuV5dnDCU/s4R0/JJTwAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMy0wOC0yMFQxMDoxODozMyswMDowMBhIJcwAAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjMtMDgtMjBUMTA6MTg6MzMrMDA6MDBpFZ1wAAAAAElFTkSuQmCC";
const blob = Utils.dataURLtoBlob(dataURL);
console.log(blob);
```

- 效果：

![将 Data URL 转换为 Blob 对象](https://static.codemao.cn/i/24/5/2/18/1620-10.png)

---