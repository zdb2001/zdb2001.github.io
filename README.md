# 一分钟上线：免费个人主页

这是一页式、纯静态的个人主页模板。你可以在 **GitHub Pages**、**Netlify** 或 **Vercel** 免费托管。

## 方案 A：GitHub Pages（最简单、零代码部署）
1. 把此仓库上传到 GitHub，并命名为：`<你的用户名>.github.io`（比如 `alice.github.io`）。
2. 把 `index.html` 放到仓库根目录并提交。
3. 打开仓库的 **Settings → Pages**，Source 选择 **Deploy from a branch**，分支选 `main`，`/root`。
4. 等 1–2 分钟，访问 `https://<你的用户名>.github.io` 即可看到主页。

## 方案 B：Netlify / Vercel（适合后续加构建）
- 直接把本仓库导入平台，Build 命令留空（因为纯静态），Publish 目录填 `.`。
- 平台会分配一个 `*.netlify.app` 或 `*.vercel.app` 域名。

## 自定义域名（可选）
- 购买域名后，在 DNS 增加 CNAME：把 `www` 指向你的 Pages/托管域名。
- GitHub Pages：在仓库根目录新建 `CNAME` 文件，写入你的域名，如 `www.example.com`。

## 个性化修改
- 文本：直接编辑 `index.html` 里的名字、项目、论文、链接。
- 颜色/风格：修改 `<style>` 中的 CSS 变量（`--accent` 等）。
- 图标：把 `avatar` 换成你的头像（可改成 `<img>`）。

## 无障碍与 SEO
- 已包含 `lang="zh-CN"`、`meta description`。
- 所有外链加 `rel="noopener"`，性能与安全更好。

祝你玩得开心！
