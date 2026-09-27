# 南通 · 江海长卷

一个南通的城市宣传页：长江入海口北翼，一座从海里长出来的城。蓝印花布 + 江海交汇的视觉，
十四个区块从成陆、近代第一城，一路走到濠河夜游、狼山、大桥、染坊、板鹞风筝、江鲜、乡音、行程与结尾海报。

- 在线访问（GitHub Pages）：<https://futurebackrookie.github.io/nantong-jianghai-changjuan/>
- 国内镜像（Cloudflare Pages）：<https://nantong-jianghai-changjuan.pages.dev/>

## 这个仓库

本仓库是**发布版**：由源码仓库的 `scripts/build-deploy.sh` 生成，`main` 分支根目录即站点。

- 只含站点文件：`index.html`、`css/`、`js/`、`vendor/`、`fonts/`、`images/`、`LICENSE`、`_headers`、`.nojekyll`。
- `js/`、`css/` 已用 esbuild 压缩（去注释、缩短变量名）；可读源码、测试与构建脚本留在源码仓库，不在这里改。
- 纯静态、完全自包含：图片、字体、动画库都在仓库里，不依赖 CDN。下载后**双击 `index.html`** 也能离线打开。
- `_headers` 让 Cloudflare Pages 对字体缓存一年（字体地址带内容指纹 `?v=`，重建字体后地址跟着变），对图片与 `vendor/` 缓存 30 天；GitHub Pages 忽略它。

## 许可

代码 MIT（见 `LICENSE`）；图片按各自的 CC 许可证或公有领域（逐张署名见页脚「图片来源与署名」）；
地图数据 ODbL；方言词条 CC BY-SA 4.0；字体 SIL Open Font License；
笔顺数据 `js/strokes/*.js` 遵循 Arphic Public License，原文 `js/strokes/ARPHICPL.TXT` 随数据分发。
详见 `LICENSE`。
