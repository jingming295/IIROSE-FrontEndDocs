# 弹出框

> 弹出框

## 函数
```javascript
Utils.sync(e, t, o)
```

```e```: 类型。0是提示框，1是验证框，2是input的输入框，3是textarea的输入框

```t```: 如果e是提示框或输入框，他是标题。在e验证框，他是内容。

```o```: 回调函数

## 提示框

> 弹出一个提示框

- 使用例子

```javascript
function test() {
  _alert(`提示回调函数`)
}
Utils.sync(0,["这是一个提示"], test)
```

- 效果：

![提示框](https://static.codemao.cn/i/24/4/17/16/0345-I2.png)

---

## 验证框

> 弹出一个验证框

- 使用例子

```javascript
function test(bool) {
  _alert(bool)
}
Utils.sync(1,["这是一条验证信息"], test)
```

如果你点击确定，那么回调函数的bool将会获得一个true的布尔值，如果点击取消，将会获得一个false的布尔值

- 效果：

![验证框](https://static.codemao.cn/i/24/4/17/16/1425-T0.png)

---

## 输入框 (input)

> 弹出一个输入框，类型是input

- 使用例子

```javascript
function test(input) {
  _alert(input)
}
Utils.sync(2,["请输入你的内容"], test)
```

如果你点击确定，那么回调函数的第一个接收值将会是input的内容 (用户的输入)，如果点击取消的话将会是null。

- 效果：

![input输入框](https://static.codemao.cn/i/24/4/17/16/2136-K7.png)

---

## 输入框 (textarea)

> 弹出一个输入框，类型是textarea，可多行

- 使用例子

```javascript
function test(input) {
  _alert(input)
}
Utils.sync(3,["请输入你的内容"], test)
```

如果你点击确定，那么回调函数的第一个接收值将会是input的内容 (用户的输入)，如果点击取消的话将会是null。

- 效果：

![textarea输入框](https://static.codemao.cn/i/24/4/17/16/2419-H7.png)

---