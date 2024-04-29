# buildPm

## Utils.buildPm(e,t,o,i,a)

> 看起来像是构建私聊信息

```javascript
Utils.buildPm(e,t,o,i,a)
```

```e```: 用户的唯一标识

```t```: t数组包含了私信消息构建所需的参数

```t[0]```: 构建私聊的时候，为私聊对象用户头像

```t[1]```: hex color值。

```t[2]```: 用户的昵称

```t[3]```: 数字，不清楚有什么用

```t[4]```: 私聊对象的私聊背景图

```o```: 对应privateMsgFunc的```r```, 为真的时候就打开私聊界面

```i```: 对应privateMsgFunc的```l```，为真的时候，如果```o```为真，但是不为```*```，就会打开私聊界面，然后对方变匿名。如果为```*```，那么你变匿名

```a```: 对应privateMsgFunc的n，还不清楚是什么

### 构建私聊信息

- 使用例子

```javascript
var e = "625874e344db0"; // 用户的唯一标识
var t = ['http://r.iirose.com/i/23/1/16/19/5713-GK.jpg#e', 'ffffa7', '用户名', '4', 'http://r.iirose.com/i/24/1/18/11/3943-HK.png']; // t数组包含了私信消息构建所需的参数
var o = 1 // 对应privateMsgFunc的r
var i = 1 // 对应privateMsgFunc的l
var a = undefined; // 对应privateMsgFunc的n

// 调用 buildPm 函数
var result = Utils.buildPm(e, t, o, i, a);
console.log(result)
```

以上代码将会使你主动为对方开启匿名聊天。

- 效果：

![打开私聊界面](https://i.imoe.xyz/uploads/01HWMP8HCN5W9AP7JVV4KSXW33.png)

![console](https://static.codemao.cn/i/24/4/29/18/2717-UK.png)

---