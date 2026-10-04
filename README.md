# 现场水印相机

一个面向安卓手机的轻量 H5 拍照工具。支持拍照或从相册选择图片，添加可编辑的日期、时间和地址水印，并在浏览器本地生成 JPG。

## 在线体验

[打开现场水印相机](https://field-watermark-camera.shenjiaping0.chatgpt.site)

## 功能

- 调用手机后置相机拍照
- 从相册选择照片
- 修改日期与时间
- 填写和恢复默认地址
- 蓝牌、黑底两种水印样式
- 左下、右下水印位置
- 在浏览器本地生成并下载 JPG
- 不读取经纬度，不主动上传照片或地址

## 本地运行

项目为纯静态网页，无需安装依赖：

```bash
python3 -m http.server 4173 --directory dist
```

然后访问 `http://127.0.0.1:4173`。

相机功能在手机浏览器中通常需要 HTTPS；本地开发时浏览器一般允许 `localhost` 使用相机。

## 修改默认地址

编辑 `dist/index.html` 中的 `DEFAULT_ADDRESS`：

```js
const DEFAULT_ADDRESS = "你的默认地址";
```

## 项目文件

- `dist/index.html`：完整网页应用
- `PRODUCT.md`：产品定义
- `DESIGN.md`：视觉设计系统
- `direction-contract.md`：本次设计方向约束
