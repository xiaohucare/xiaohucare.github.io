# 小护康养 mini · 官网静态站

[xiaohucare.github.io](https://xiaohucare.github.io) 的源码仓库，纯静态页面，通过 GitHub Pages 自动部署（见 `.github/workflows/static.yml`）。

## 页面说明

| 文件 | 说明 |
| --- | --- |
| `index.html` | 项目介绍首页：模块能力、技术栈、快速开始、开源信息、商务咨询（Vue 3 + Element Plus CDN 引入） |
| `zhihuizoom.html` | 智慧园区大屏展示页：全屏展示 `park-screen.png`，顶部带与首页一致的导航 |

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
