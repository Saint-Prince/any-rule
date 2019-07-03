# any-rule 
正则大全
https://any86.github.io/any-rule/

## 银行卡号（16或19位）
```javascript
/^([1-9]{1})(\d{15}|\d{18})$/
```

## 中文姓名
```javascript
/^([\u4e00-\u9fa5·]{2,10})$/
```

## 新能源车牌号
```javascript
/[京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼使领 A-Z]{1}[A-HJ-NP-Z]{1}(([0-9]{5}[DF])|([DF][A-HJ-NP-Z0-9][0-9]{4}))$/
```

## 非新能源车牌号
```javascript
/^[京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼使领 A-Z]{1}[A-HJ-NP-Z]{1}[A-Z0-9]{4}[A-Z0-9挂学警港澳]{1}$/
```

## 车牌号(新能源+非新能源)
```javascript
/^([京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼使领 A-Z]{1}[A-HJ-NP-Z]{1}(([0-9]{5}[DF])|([DF]([A-HJ-NP-Z0-9])[0-9]{4})))|([京津沪渝冀豫云辽黑湘皖鲁新苏浙赣鄂桂甘晋蒙陕吉闽贵粤青藏川宁琼使领 A-Z]{1}[A-Z]{1}[A-HJ-NP-Z0-9]{4}[A-HJ-NP-Z0-9 挂学警港澳]{1})$/
```

## URL链接
```javascript
/^((https?|ftp|file):\/\/)?([\da-z.-]+)\.([a-z.]{2,6})(\/\w\.-]*)*\/?$/
```

## 手机号
```javascript
/^1((3[\d])|(4[5,6,7,9])|(5[0-3,5-9])|(6[5-7])|(7[0-8])|(8[\d])|(9[1,8,9]))\d{8}$/
```

## 大写字母
```javascript
/^[A-Z]+$/
```

## 日期,如: 2000-01-01
```javascript
/^\d{4}(-)\d{1,2}\1\d{1,2}$/
```

## email地址
```javascript
/^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$/
```

## 国内座机电话,如: 0341-86091234
```javascript
/\d{3}-\d{8}|\d{4}-\d{7}/
```

## 身份证号(15位、18位数字)，最后一位是校验位，可能为数字或字符X
```javascript
/(^\d{15}$)|(^\d{18}$)|(^\d{17}(\d|X|x)$)/
```

## 帐号是否合法(字母开头，允许5-16字节，允许字母数字下划线组合
```javascript
/^[a-zA-Z][a-zA-Z0-9_]{4,15}$/
```

## 只包含中文
```javascript
/^[\u4E00-\u9FA5]+$/
```

## 是否小数
```javascript
/^\d+\.\d+$/
```

## 是否电话格式(手机和座机)
```javascript
/^((0\d{2,3}-\d{7,8})|(1[345789]\d{9}))$/
```

## 是否8位纯数字
```javascript
/^[0-9]{8}$/
```

## 是否html标签
```javascript
/<(.*)>.*<\/\1>|<(.*) \/>/
```

## 是否qq号格式正确
```javascript
/^[1-9][0-9]{4,10}$/
```

## 是否由数字和字母组成
```javascript
/^[A-Za-z0-9]+$/
```

## 是否小写字母组成
```javascript
/^[a-z]+$/
```

## 密码强度正则，最少6位，包括至少1个大写字母，1个小写字母，1个数字，1个特殊字符
```javascript
/^.*(?=.{6,})(?=.*\d)(?=.*[A-Z])(?=.*[a-z])(?=.*[!@#$%^&*? ]).*$/
```

## 用户名正则，4到16位（字母，数字，下划线，减号）
```javascript
/^[a-zA-Z0-9_-]{4,16}$/
```

## ipv4地址正则
```javascript
/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/
```

## 16进制颜色
```javascript
/^#?([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$/
```

## 微信号，6至20位，以字母开头，字母，数字，减号，下划线
```javascript
/^[a-zA-Z]([-_a-zA-Z0-9]{5,19})+$/
```

## 中国邮政编码
```javascript
/^(0[1-7]|1[0-356]|2[0-7]|3[0-6]|4[0-7]|5[1-7]|6[1-7]|7[0-5]|8[013-6])\d{4}$/
```

## 只包含中文和数字
```javascript
/^(([\u4E00-\u9FA5])|(\d))+$/
```

## 非字母
```javascript
/[^A-Za-z]$/
```
