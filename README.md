# base64-decoding
无依赖utf8字符base64编/解码模块，可安全用于微信小程序(不建议在用于生产环境,更不更新看心情,仅仅想温故一下js)

## 安装
### nodejs方式安装
```
npm install base64-decoding --save
```

### bower方式安装
```
bower install base64-decoding
```

## 用法
### require方式
```javascript
var base64 = require('base64-decoding');

var str = "base64中文字符测试";
var encodeString = base64.encode(str); // 编码
var decodeString = base64.decode(encodeString); // 解码

console.log(encodeString); // YmFzZTY05Lit5paH5a2X56ym5rWL6K+V
console.log(decodeString); // base64中文字符测试
```

### 引入方式
```html
<script src="bower_components/base64-decoding/dist/base64.min.js"></script>
<script>
var str = "base64中文字符测试";
var encodeString = base64.encode(str); // 编码
var decodeString = base64.decode(encodeString); // 解码

console.log(encodeString); // YmFzZTY05Lit5paH5a2X56ym5rWL6K+V
console.log(decodeString); // base64中文字符测试
</script>
```