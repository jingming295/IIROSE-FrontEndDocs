# copyData

## Utils.copyData(e)

> 复制文本

```javascript
Utils.copyData(e)
```

```e```: 文本，想要复制的文本

- 当```device```为5，并且具有 Main.putClipboardData 函数时，它会调用 Main.putClipboardData(e) 来执行复制操作，并返回 true 表示复制成功。
- 对于其他，它会先将文本数据放入一个隐藏的 DOM 元素（Objs.repertory.contentCopyHolder）中，并尝试使用 document.execCommand("copy") 来触发浏览器的复制命令。在这之前，它先获取了当前文档的选区对象 getSelection()，然后创建了一个范围对象 document.createRange()，并将范围设置为文本元素的内容。接着调用 document.execCommand("copy") 方法尝试复制文本到剪贴板。最后，它返回复制操作的结果（成功或失败）。

### 复制文本

- 使用例子

```javascript
const result = Utils.copyData("要复制的文本数据");
console.log(result)
```

- 效果：

![判断](https://static.codemao.cn/i/24/5/1/23/5050-YC.png)

---