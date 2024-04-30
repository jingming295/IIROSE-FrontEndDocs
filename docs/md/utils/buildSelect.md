# buildSelect

## Utils.buildSelect(i,a,s,r,e,t,o,l,n)

> 创建选择框（第一种）

```javascript
Utils.buildSelect(i,a,s,r,e,t,o,l,n)
```

```i```: htmlElement，传入这个是为了当用户选择选项的时候，把选项的text替换到i的innerHTML。如果```i```有```setAttribute('v')```，那么v的，比如说```"0,1,,3"```就是多选，并且0, 1, 3已选。如果```i```有```setAttribute('data-checkbox')```，那么本来单选框会变多选框

```a```: 2D数组，结构为类似 ```[[0, "选项1", "htmlElement"], [1, "选项2", "htmlElement"]]```

```s```: 回调函数

```r```: htmlElement，如果这个有值，那么用户选择后，将会把选择的text变为这个element的innerHTML

```e```: 是否显示图标，如果显示，则用a[i][2]的htmlElement显示

```t```: 是文本，将会出现在选择框的顶端

```o```: 是文本，将会出现在选择框的底端

```l```: 如果不选择，返回的时候的回调函数

```n```: 是否允许选择空值（未经验证）


### 创建选择框（第一种）

- 使用例子

```javascript

const a = [
    [0, '选项1', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`],
    [1, '选项2', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`],
    [2, '选项3', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`],
    [3, '选项4', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`]
]

function s(t, s) {
    console.log("用户选择了选项：", s);
}

function l(){
    console.log("用户按下了回车")
}

var elements = document.getElementsByClassName('room_chat_content');
var i = elements[elements.length - 1];
var r = elements[elements.length - 2];
i.setAttribute("v", "0,1,,3"); // 这里假设选择了选项 0、1、2
i.setAttribute("data-checkbox", '')
Utils.buildSelect(i, a, s, r, true, '这是顶层', '这是底层', l, true)

```

- 效果：

![打开选择框](https://static.codemao.cn/i/24/4/30/13/4241-VL.png)

![回调函数输出](https://static.codemao.cn/i/24/4/30/13/4320-28.png)

---