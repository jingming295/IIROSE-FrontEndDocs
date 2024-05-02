# demandGetDef

## Utils.demandGetDef(e)

> 获取对应的视频分辨率信息

```javascript
Utils.demandGetDef(e,t)
```

```e```: 数字，用来确定返回的是哪个视频站的分辨率信息

```t```: 文本，影响到返回的描述信息

|```e```|对应选项|```t```的可用值
|:--:|--|--|
|0|分辨率信息|0，1，2，3，4，5，6，10，14，17，18，19，21，96|
|1|分辨率信息|1，2，3，4，mp4|
|2|Youtube视频的分辨率信息,|1，2，3，4，5，6，9|
|3|B站视频的分辨率信息|2，3，4，16，32，64，74，80，112，116|
|8|B站直播的分辨率信息|80，150，250，400，1e4，2e4，3e4|
|100|分辨率信息|```t```可以为1，2，3|

### 获取对应的视频分辨率信息

- 使用例子

```javascript
let description = Utils.demandGetDef(1, '1');
console.log(description);
```

- 效果：

![分辨率信息](https://static.codemao.cn/i/24/5/3/0/4846-VY.png)

---