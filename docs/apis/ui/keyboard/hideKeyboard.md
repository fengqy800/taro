---
title: Taro.hideKeyboard(option)
sidebar_label: hideKeyboard
---

在input、textarea等focus拉起键盘之后，手动调用此接口收起键盘

> [参考文档](https://developers.weixin.qq.com/minigame/dev/api/ui/keyboard/wx.hideKeyboard.html)

## 类型

```tsx
(option?: Option) => void
```

## 参数

### Option

| 参数 | 类型 | 必填 | 说明 |
| --- | --- | :---: | --- |
| complete | `(res: CallbackResult) => void` | 否 | 接口调用结束的回调函数（调用成功、失败都会执行） |
| fail | `(res: CallbackResult) => void` | 否 | 接口调用失败的回调函数 |
| success | `(res: CallbackResult) => void` | 否 | 接口调用成功的回调函数 |

## 示例代码

```tsx
Taro.hideKeyboard({
  complete: res => {
    console.log('hideKeyboard res', res)
  }
})
```

## API 支持度

| API | 微信小程序 | H5 | React Native |
| :---: | :---: | :---: | :---: |
| Taro.hideKeyboard | ✔️ |  |  |
