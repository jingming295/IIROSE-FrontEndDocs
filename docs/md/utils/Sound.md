# Sound

## Utils.Sound.gameAudioPlayer(e, t)

> 播放提示音

```javascript
Utils.Sound.gameAudioPlayer(e, t)
```

```e```: 数字, 可以为1 - 9

```t```: 文本，如果```e```为9的时候，将会使用t的文本，和``` https://static.codemao.cn/rose/v0/lib/system/sound/effect/e.mp3```组合获取音效然后播放


### 播放提示音

- 使用例子

```javascript
Utils.Sound.gameAudioPlayer(2);
```

---

## Utils.Sound.onmousedown(e)

> 当点击的时候播放音效
> 还没完全搞清楚怎么使用

```javascript
Utils.Sound.onmousedown(e)
```

```e```: MouseEvent，好像也可以传htmlelement


### 当点击的时候播放音效

- 使用例子

```javascript
Utils.Sound.onmousedown(mouseEvent)
```

---

## Utils.Sound.play(e, t)

> 播放提示音

```javascript
Utils.Sound.play(e, t)
```

```e```: 数字, 可以为1 - 9

```t```: 文本，如果```e```为9的时候，将会使用t的文本，和``` https://static.codemao.cn/rose/v0/lib/system/sound/effect/e.mp3```组合获取音效然后播放

在播放之前，该函数会检查一些条件：

- 如果 Probe.skipSound 为真，则跳过播放提示音。

- 如果 Probe.muteEffectSound 为真，则跳过播放提示音。

- 如果 Probe.initshowOverLive 为真且不处于睡眠模式下，则继续执行播放音频的操作。

- 此外，还会检查 Probe.changeSound 的值，如果为真且 e 为 3，则将 e 的值修改为 2。

- 最后，调用 gameAudioPlayer 函数来播放音频，传入参数 e 和 t。

### 播放提示音

- 使用例子

```javascript
Utils.Sound.play(2);
```
