# compareScroll

## Utils.compareScroll(e,t)

> 判断一个元素是否已经滚动到了其内容的底部（我不确定是不是这样）

```javascript
Utils.compareScroll(e,t)
```

```e```: Html元素

```t```: 偏移量

### 判断一个元素是否已经滚动到了其内容的底部

- 使用例子

```javascript
const homeHolderMsgBox = document.getElementsByClassName('homeHolderMsgBox');
const secondElement = homeHolderMsgBox[1];
const isScrolled = Utils.compareScroll(secondElement, 800);
console.log(isScrolled);
```

- 效果：

![判断](https://static.codemao.cn/i/24/4/30/19/2745-XY.png)

---