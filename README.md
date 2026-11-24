# 小护康养 mini · 官网静态站

[xiaohucare.github.io](https://xiaohucare.github.io) 的源码仓库，纯静态页面，通过 GitHub Pages 自动部署（见 `.github/workflows/static.yml`）。

## 页面说明

| 文件 | 说明 |
| --- | --- |
| `index.html` | 项目介绍首页：模块能力、技术栈、快速开始、开源信息、商务咨询（Vue 3 + Element Plus CDN 引入） |
| `zhihuizoom.html` | 智慧园区大屏展示页：全屏展示 `park-screen.png`（`park-screen.jpg` 为压缩版，浏览器优先加载），顶部带与首页一致的导航 |
| `robots.txt` / `sitemap.xml` | 搜索引擎抓取规则与站点地图，域名统一使用 <https://xiaohucare.com> |
| `og-cover.jpg` | 社交分享卡片配图（1200×630），用于 Open Graph / Twitter Card |

## SEO 要点

- 全站 canonical 指向 `https://xiaohucare.com/`（`xiaohucare.github.io` 会 301 跳转到该域名），改版时同步修改 `index.html`、`zhihuizoom.html` 与 `sitemap.xml`。
- 首页为 Vue 3 客户端渲染，因此 `<div id="app">` 内保留了一份静态正文（`.seo-fallback`），供不执行 JS 的爬虫与弱网环境读取；Vue 挂载后会自动替换，不影响正常用户。
- 已内置 description / keywords、Open Graph、JSON-LD 结构化数据（WebSite、Organization、SoftwareApplication）。

## 本地运行

```bash
python3 -m http.server 8080
```

浏览器访问 <http://localhost:8080> 即可。

## 相关仓库

- 前端（Vue 3）：[xiaohucare/xiaohucare-mini-vue](https://github.com/xiaohucare/xiaohucare-mini-vue) · [Gitee 镜像](https://gitee.com/chongkelai/xiaohucare-mini-vue)
- 后端（Java）：[xiaohucare/xiaohucare-mini](https://github.com/xiaohucare/xiaohucare-mini) · [Gitee 镜像](https://gitee.com/chongkelai/xiaohucare-mini)

## 许可

MIT License
