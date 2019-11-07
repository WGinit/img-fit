<!--
 * @Author: wginit
 * @Date: 2019-11-06 14:18:53
 * @LastEditTime: 2019-11-07 09:30:51
 -->
# Web端图片自适应显示

> 思路来自于小程序image组件

### 如何使用

> 传统引入

```javascript
<script src="./lib/index.js"></script>
```

> npm 引入

```javascript
npm i img-fit

require('img-fit')
```
### 示例

```javascript
<img src="../sheep.png" mode="scaleToFill" />
```

### img参数

| 参数    | 类型   |  默认值  |  必填  |  说明 |
| :----: | :-----:  | :----:  |  :--: |  :---: |
| mode | String | '' | N | 显示类型，详情见以下描述 |
| width | String | 300px | N | 宽度|
| height | String | 220px | N | 高度 |
| error | Function | null | N | 加载失败 |

#### mode 参数
| 字段 | 说明|
| :---: | :---: |
| scaleToFill | 缩放模式，不保持纵横比缩放图片，使图片的宽高完全拉伸至填满 img 元素 |
|aspectFit | 缩放模式，保持纵横比缩放图片，使图片的长边能完全显示出来。也就是说，可以完整地将图片显示出来。|
|aspectFill| 缩放模式，保持纵横比缩放图片，只保证图片的短边能完全显示出来。也就是说，图片通常只在水平或垂直方向是完整的，另一个方向将会发生截取。|
| widthFix | 缩放模式，宽度不变，高度自动变化，保持原图宽高比不变|
| top| 裁剪模式，不缩放图片，只显示图片的顶部区域|
| bottom| 裁剪模式，不缩放图片，只显示图片的底部区域|
| center | 裁剪模式，不缩放图片，只显示图片的中间区域|
| left | 裁剪模式，不缩放图片，只显示图片的左边区域 |
| right | 裁剪模式，不缩放图片，只显示图片的右边区域 |
| topLeft | 裁剪模式，不缩放图片，只显示图片的左上边区域 |
| topRight | 裁剪模式，不缩放图片，只显示图片的右上边区域 |
|bottomLeft | 裁剪模式，不缩放图片，只显示图片的左下边区域 |
| bottomRight | 裁剪模式，不缩放图片，只显示图片的右下边区域 |

### 效果展示

原图

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/sheep.png)

scaleToFill

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/1.png)

aspectFit

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/2.png)

aspectFill

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/3.png)

widthFix

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/4.png)

top

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/5.png)

bottom

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/6.png)

center

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/7.png)

left

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/8.png)

right

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/9.png)

topLeft

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/10.png)

topRight

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/11.png)

bottomLeft

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/12.png)

bottomRight

![image](https://raw.githubusercontent.com/WGinit/Assets/master/project/images/img-fit/13.png)

