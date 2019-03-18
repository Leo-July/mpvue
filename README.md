# 小程序

1、去掉 button 默认 border

```css
.button::after {
  border: none;
}
```

# mpvue

1、button 获取手机号

```html
<button
  open-type="getPhoneNumber"
  @getphonenumber="getContact">获取手机号</button>
```
```js
getContact(e){
  console.log(e.mp.detail.encryptedData)
  console.log(e.mp.detail.iv)
  console.log(e.mp.detail.errMsg)
}
```
2、`image`标签，安卓手机图片无法显示   
`src`属性如果非本地图片必须是带有协议的地址
