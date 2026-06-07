# FREE LIGHTING Website

英文公司官网 for FREE LIGHTING — Shenzhen LED bulb & dimmer manufacturer.
纯静态网站（HTML/CSS/JS），无需构建。

## 本地预览

方式一：直接双击 `index.html`。

方式二（推荐，链接更准确）：在项目根目录运行
```bash
python -m http.server 8000
```
然后浏览器打开 http://localhost:8000

## 结构
- `index.html` — 首页
- `about.html` — 公司介绍
- `products.html` — 产品总览
- `products/g4.html` · `g9.html` · `gu10.html` — 三款产品
- `contact.html` — 联系
- `assets/css/style.css` · `assets/js/main.js` — 全站样式与脚本
- `网站素材/` — 数据来源（不参与网站运行）

## 说明
- 产品仅展示 G4 / G9 / GU10 三款
- 产品图片引用 freelightingled.com 远程地址
- 联系表单为前端 UI，提交走 WhatsApp / 邮件（无后端）

详细约定见 `CLAUDE.md`。
