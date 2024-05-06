# AppUtils

## Utils.AppUtils.getShareData()

> 解析文本

```javascript
Utils.AppUtils.getShareData()
```

### 弹出解析文本的选择框

- 使用例子

```javascript
var Main = {
    getShareData: function() {
        return "这是\n文本";
    }
};
Utils.AppUtils.getShareData()
```

你需要先定义一个Main的对象，里面有个getShareData返回string。调用后，他会弹出解析文本的控件

- 效果：

![解析文本](https://static.codemao.cn/i/24/4/17/17/5120-ZA.png)

---

## Utils.AppUtils.menu

> 处理图片

```javascript
Utils.AppUtils.menu(e,o)
```

```e```: 有两个可用的值，1_0_为呼出包含**设为壁纸**的选择框，1_0为不包含**设为壁纸**的选择框
```o```: 是string，为图片的网址

### 弹出处理图片的选择框

- 使用例子

```javascript
Utils.AppUtils.menu('1_0_','http://r.iirose.com/i/21/10/19/20/1347-OZ.jpg#e')
```

- 效果：

![解析文本](https://static.codemao.cn/i/24/4/17/21/3947-ZD.png)

---

## Utils.AppUtils.setCoreType

> 还没有完全搞清楚这是干什么的。貌似是备份数据，储存到localstorage，他好像是应该在保存成功后重启蔷薇花园

```javascript
Utils.AppUtils.setCoreType(t)
```

```t```: 不确定是什么值，不确定是干什么的

### 备份数据(不确定)

- 使用例子

```javascript
var Main = {
    setData: function(key, value, callback) {
        // 模拟保存数据
        console.log("key:", key);
        console.log("value", value)
        // 模拟异步操作，这里直接调用回调函数
        callback();
    },
    restartApp: function() {
        // 模拟重启应用
        console.log("Restarting app...");
    }
};

// 使用 Utils.AppUtils.setCoreType
Utils.AppUtils.setCoreType("some_value");
```

- 效果：

![解析文本](http://r.iirose.com/i/24/4/17/22/1653-D8.png)