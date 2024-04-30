# buildSelect2

## Utils.buildSelect2(i,a,s,e,t,o,r,l,n)

> 创建选择框（第一种）

```javascript
Utils.buildSelect2(i,a,s,e,t,o,r,l,n)
```

```i```: htmlElement，作为选择选项后，作为回调函数的第一个参数

```a```: 2D数组，结构为类似 ```[[0, "选项1", "HTML字符串"], [1, "选项2", "HTML字符串"]]```

```s```: 回调函数

```e```: 是否禁止清空选项 (禁止点空白的地方返回)

```t```: 是否显示图标

```o```: 自定义HTML字符串，出现在顶端

```r```: 是否启用多选功能

```l```: 自定义HTML字符串，出现在底端

```n```: 返回（点击空白处）的回调函数


### 创建选择框（第一种）

- 使用例子

```javascript

const a = [
    [0, '选项1', `<div class="mdi-badge-account-horizontal" style="font-family:md;font-size:28px;text-align:center;line-height:100px;height:100px;width:100px;position:absolute;top:0;opacity:.7;left:0;"></div>`],
    [1, '选项2', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`],
    [2, '选项3', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`],
    [3, '选项4', `<div style="height:100px;width:100px;position:absolute;top:0;left:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/24/1/19/1/5954-6L.jpg#e" onerror="this.style.display='none';"><div class="fullBox"></div></div></div>`]
]

function s(t, s) {
    console.log("用户选择了选项：", s);
}

function n(){
    console.log("用户按下了回车")
}

var elements = document.getElementsByClassName('room_chat_content');
var i = elements[elements.length - 1];
var r = true; // 是否启用多选
var e = true; // 是否禁止清空选项 (禁止点空白的地方返回)
var t = true; // 是否显示图标
var o = `<div onclick="event.stopPropagation();" style="height:100px;width:100%;position:relative;box-shadow:0 0 1px rgba(0,0,0,0.12),0 1px 1px rgba(0,0,0,0.24);overflow:hidden;background-color:#ffffff;color:rgba(0,0,0,0.75);"><div class="selectHolderBoxItem textOverflowEllipsis" style="padding-left:48px;padding-right:124px;position:absolute;white-space:nowrap;"><div class="mapHolderRoomUserMenuBoxItemInfoStatus" style="background-color:#43b581;box-sizing:border-box;border:1px solid rgba(0,0,0,0.75);height:16px;width:16px;margin-top:10px;margin-right:12px;"></div><span style="font-size:inherit;font-weight:inherit;white-space:pre;">铭_<span style="margin-left:12px;font-size:14px;font-weight:bold;opacity:.7;position:relative;top:7px;border-radius:2px;border:1px solid rgba(0,0,0,.5);padding:0 8px;line-height:22px;vertical-align:top;">_<span style="opacity:.3;margin:0 6px;font-size:inherit;">/</span><span style="font-family:md;font-size:inherit;opacity:.75;" class="mdi-code-braces"></span>  开发者</span></span><span style="font-weight:bold;font-size:12px;line-height:36px;white-space:pre;position:absolute;bottom:2px;left:48px;right:100px;"><span style="opacity:.8;"><span style="border-radius:2px;background:#4EBBF9;color:#202020;padding:0 8px;line-height:20px;height:20px;display:inline-block;margin-right:12px;"><span class="mdi-gender-male" style="font-family:md;font-weight:100;font-size:14px;vertical-align:top;"></span></span><span style="border-radius:2px;background:#43b581;color:#fff;padding:0 8px;line-height:20px;height:20px;display:inline-block;">聊天中</span><span style="opacity:.7;border-radius:2px;background:#202020;color:#fff;padding:0 8px;line-height:20px;height:20px;display:inline-block;margin-left:12px;"><span class="mdi-hexagon-slice-2" style="font-family:md;font-weight:100;font-size:14px;vertical-align:top;"></span>   3710  小时</span><span style="opacity:.8;border-radius:2px;background:#202020;color:#fff;padding:0 8px;line-height:20px;height:20px;display:inline-block;margin-left:12px;"><span class="mdi-account-star" style="font-family:md;font-weight:100;font-size:14px;vertical-align:top;"></span></span></span></span></div><div style="height:100px;width:100px;position:absolute;top:0;right:0;"><div class="bgImgBox"><img class="bgImg" loading="lazy" decoding="async" src="http://r.iirose.com/i/23/12/10/4/3640-Z1.jpg" onerror="this.style.display='none';"><div class="fullBox"></div></div><div style="background-image:-webkit-linear-gradient(left,#ffffff,transparent);height:100%;width:50%;position:relative;left:-1px;"></div></div></div>`
Utils.buildSelect2(i, a, s, e, t, o, r, '这是底层', n)

```

- 效果：

![打开选择框](https://static.codemao.cn/i/24/4/30/18/5122-F4.png)

![回调函数输出](https://static.codemao.cn/i/24/4/30/18/5146-P0.png)

---