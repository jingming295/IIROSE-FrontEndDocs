# database

## Utils.database(e,t)

> Assets.database的内容操作

```javascript
Utils.database(e,t)
```

```e```: 为```Assets.database```的key 

```t```: 如果有提供，那```Assets.database[e]```的内容变成```t```

### Assets.database的内容操作

- 使用例子

```javascript
console.log(Utils.database('key'))
Utils.database('key', '内容');
console.log(Utils.database('key'))
```

如果重载网页或者app后，内容不会丢失。

- 效果：

![Assets.database的内容操作](https://static.codemao.cn/i/24/5/2/19/3447-OC.png)

---