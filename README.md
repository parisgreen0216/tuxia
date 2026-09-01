# 图匣 · Page Image Folders

把网页上的图片收进文件夹。按用途、格式或尺寸整理，再打包下载。

![图匣](https://img.shields.io/badge/图匣-Page%20Image%20Folders-black)

## 功能

- 粘贴任意网页地址，自动收集页面中的图片
- 支持 `<img>`、`srcset`、懒加载属性、`background-image`、`og:image` 等
- **按格式**整理（PNG / JPG / WebP / GIF / SVG …）
- **按尺寸**整理（超大 / 大 / 中 / 小 / 极小）
- **按用途**整理（内容图片 / Logo / 图标）
- 勾选需要的图片，一键打包成 ZIP 下载
- 纯前端运行，无需安装

## 使用

直接打开 [在线演示](https://parisgreen0216.github.io/tuxia/) 或本地打开 `index.html`。

1. 粘贴网页地址（例如 `wikipedia.org`）
2. 点击「开始收图」
3. 在结果页按需筛选、勾选
4. 点击「打包下载」

> 部分网站用 JavaScript 动态加载图片，只能收到写在 HTML 里的图。跨域限制也可能导致部分图片无法预览或下载。

## 本地运行

```bash
# 任意静态服务器即可
npx serve .
# 或
python -m http.server 8080
```

## 技术

- 纯 HTML / CSS / JavaScript
- [JSZip](https://stuk.github.io/jszip/) + FileSaver 打包下载
- 使用 [allorigins](https://allorigins.win) 作为 CORS 代理（可选）

## 项目结构

```
tuxia/
├── index.html    # 页面
├── style.css     # 样式
├── app.js        # 逻辑
└── README.md
```

## License

MIT
