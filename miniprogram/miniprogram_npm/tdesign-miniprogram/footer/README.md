---
title: Footer 页脚
description: 用于基础列表展示，可附带文字、品牌 logo、操作，常用商详、个人中心、设置等页面。
spline: data
isComponent: true
---

<span class="coverages-badge" style="margin-right: 10px"><img src="https://img.shields.io/badge/coverages%3A%20lines-100%25-blue" /></span><span class="coverages-badge" style="margin-right: 10px"><img src="https://img.shields.io/badge/coverages%3A%20functions-100%25-blue" /></span><span class="coverages-badge" style="margin-right: 10px"><img src="https://img.shields.io/badge/coverages%3A%20statements-100%25-blue" /></span><span class="coverages-badge" style="margin-right: 10px"><img src="https://img.shields.io/badge/coverages%3A%20branches-100%25-blue" /></span>
## 引入

全局引入，在 miniprogram 根目录下的`app.json`中配置，局部引入，在需要引入的页面或组件的`index.json`中配置。

```json
"usingComponents": {
  "t-footer": "tdesign-miniprogram/footer/footer"
}
```

## 代码演示


<img src="https://tdesign.gtimg.com/miniprogram/readme/footer.png" width="375px" height="50%">

### 类型

基础页脚

{{ base }}

基础加链接页脚

{{ link }}

品牌页脚

{{ logo }}

## API
### Footer Props

名称 | 类型 | 默认值 | 说明 | 必传
-- | -- | -- | -- | --
copyright | String | '' | 已废弃。版权信息，type 为`text`生效 | N
text | String | '' | `1.0.0` 版权信息。 | N
logo | Object | - | 图标配置。`logo.icon` 表示图标链接地址，`logo.title` 表示标题文本，`logo.url` 表示链接跳转地址。TS 类型：`FooterLogo` `interface FooterLogo { icon: string; title?: string; titleUrl?: string }`。[详细类型定义](https://github.com/Tencent/tdesign-miniprogram/tree/develop/src/footer/type.ts) | N
text-link-list | Array | [] | 已废弃。链接列表，type 为`text`生效。name 表示链接名称， url 表示链接 page 路径，目前只支持小程序内部跳转，openType 表示跳转方式。TS 类型：`Array<LinkObj>` `interface LinkObj { name: string; url?: string; openType?: 'navigate' \| 'redirect' \| 'relaunch' \| 'switchTab' \| 'navigateBack' }`。[详细类型定义](https://github.com/Tencent/tdesign-miniprogram/tree/develop/src/footer/type.ts) | N
links| Array | [] | `1.0.0` 链接列表。name 表示链接名称， url 表示链接 page 路径，目前只支持小程序内部跳转，openType 表示跳转方式。TS 类型：`Array<LinkObj>` `interface LinkObj { name: string; url?: string; openType?: 'navigate' \| 'redirect' \| 'relaunch' \| 'switchTab' \| 'navigateBack' }`。[详细类型定义](https://github.com/Tencent/tdesign-miniprogram/tree/develop/src/footer/type.ts) | N
theme | String | 'text' | 已废弃。页脚展示类型。可选项：text/logo | N


### CSS 变量
组件提供了下列 CSS 变量，可用于自定义样式。
名称 | 默认值 | 描述 
-- | -- | --
--td-footer-link-color | @brand-color | - 
--td-footer-link-dividing-line-color | @font-gray-3 | - 
--td-footer-link-dividing-line-padding | @spacer-1 | - 
--td-footer-link-font-size | @font-size-s | - 
--td-footer-link-line-height | 40rpx | - 
--td-footer-logo-icon-height | 48rpx | - 
--td-footer-logo-icon-margin-right | @spacer | - 
--td-footer-logo-icon-width | 48rpx | - 
--td-footer-logo-title-font-size | @font-size-m | - 
--td-footer-logo-title-line-height | 48rpx | - 
--td-footer-logo-title-url-width | 256rpx | - 
--td-footer-text-color | @font-gray-3 | - 
--td-footer-text-font-size | @font-size-s | - 
--td-footer-text-line-height | 40rpx | - 
--td-footer-text-margin-top | 8rpx | - 
