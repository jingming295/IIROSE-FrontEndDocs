# deepCopy

## Utils.deepCopy(e)

> 创建对象的深层副本

```javascript
Utils.deepCopy(e)
```

```e```: 对象

### 创建对象的深层副本

- 使用例子

```javascript
let obj = {
    a: 1,
    b: {
        c: 2,
        d: {
            e: 3
        }
    }
};

let objCopy = Utils.deepCopy(obj);
console.log(objCopy)
```

在编程中，有时我们需要操作对象的副本而不影响原始对象。使用深层副本函数可以确保我们操作的是一个全新的对象，而不是原始对象的引用。

- 效果：

![Assets.database的内容操作](https://static.codemao.cn/i/24/5/3/0/1939-BZ.png)

---