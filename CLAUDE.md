# FREE LIGHTING 官网项目

FREE LIGHTING（深圳 LED 灯泡 / 调光器厂商，freelightingled.com）的英文公司官网。
纯静态网站，无构建步骤。

## 技术栈
- 纯 HTML + CSS + 原生 JavaScript，无框架、无打包工具
- 双击 HTML 即可预览；或 `python -m http.server 8000` 起本地服务器

## 目录约定（什么放哪）
```
/                  根目录放顶级页面（index/about/products/contact）
products/          各产品分类页（g4 / g9 / gu10）
assets/css/        全站样式，统一用 style.css
assets/js/         全站脚本，统一用 main.js
网站素材/          数据来源（中文 markdown），只读，不在网站中引用
```

## 命名约定
- 文件名全小写、用连字符（kebab-case），如 `g4.html`
- CSS class 用 kebab-case，遵循现有命名（`.site-nav` `.product-card` `.spec-table`）
- 页面语言：英文（外贸站，面向海外客户）

## 数据来源
- 所有公司信息、产品规格、图片 URL 均取自 `网站素材/` 下的 markdown
- 产品只展示 **G4、G9、GU10** 三款
- GU10 数据见 `网站素材/产品-GU10灯泡.md`（含 AR70 宽光束款）
- 图片直接引用 freelightingled.com 远程 URL，不下载到本地

## 设计系统
- 现代简洁工业风：深色基底 + 琥珀金高亮（#FFB627）
- 配色/排版/组件定义集中在 `assets/css/style.css` 顶部的 `:root` 变量
- 改样式优先改变量，不要散落硬编码颜色

## 工程纪律
- 改完页面后起本地服务器逐页验证：导航、数据、图片加载、响应式、内部链接无 404
- 不臆造产品数据，一切以素材为准
- 新增页面时复用现有导航/页脚结构，保持各页一致
