# infiniteDropdown

infinite dropdown

[DOCUMENT](https://lwxyfer.github.io/infinitedropdown/)

# USAGE

## Installation

USE npm: `npm install --save infinitedropdown`

## Usage

simply include
```js
<script src="/path/to/infinitedropdown.min.js">
```
or

if you use webpack or module loaders:
```js
// CommonJS
var idd = require('infinitedropdown');

// ES2015
import idd from 'infinitedropdown';
```

config:
```js
var idd = infinitedropdown({
  selector = '.am-idd', // required 默认.am-idd
  data = false, // required 指定载入的数据
  init = false, // required 数据初始位置
  showTooltip = true, // optional 是否显示指示信息
  tooltip = '请设置提示信息', // optional 替换默认的提示信息
  defaultValue = false, // optional 下拉框设定默认值
  className = '', // optional 给select增加样式名
  callback = false, // optional 设置回调函数，每次选择后触发回调函数
  })
```
html:
```html
<div class="am-idd"></div>
```

## required data structure

data structure like hash(structure is simple and clear)

```js
const data = {
  1: {
    10: '水果',
    20: '蔬菜',
  },
  10: {
    100: '苹果',
    101: '香蕉',
  },
  20: {
    200: '土豆',
    201: '大蒜',
    202: '茄子',
  },
  100: {
    1000: '苹果一种',
    1001: '苹果两种',
  },
  101: {
    1010: '香蕉1',
    1011: '香蕉2',
  },
}
```
## MIT LICENSE
