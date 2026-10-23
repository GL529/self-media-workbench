# AI 自媒体教练 / 编导工作台

一个纯前端、无需后端的自媒体创作辅助工作台，支持赛道自测、每日选题、脚本生成、评论区分析、爆款知识库、视频精剪、商业变现七大模块。

## 快速部署（任选一种）

### 方式一：Netlify（推荐，最简单）

1. 打开 [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. 把 `self-media-workbench-deploy` 整个文件夹**拖拽**到网页中
3. 等待几秒，Netlify 会自动生成一个公开链接
4. 把链接保存到手机/电脑浏览器书签，即可随时随地访问

> 免费额度足够个人使用，支持自定义域名。

### 方式二：Vercel

1. 打开 [https://vercel.com/new](https://vercel.com/new)
2. 选择 Import Git Repository（如果你会 Git）或直接使用 Vercel CLI
3. 上传本文件夹内容
4. 部署完成后获得 `https://你的项目名.vercel.app` 链接

### 方式三：GitHub Pages（免费、长期稳定）

1. 在 GitHub 新建一个仓库，例如 `self-media-workbench`
2. 把本文件夹里的 `index.html` 上传到仓库根目录
3. 进入仓库 Settings → Pages → Source 选择 `main` 分支
4. 等待 1-2 分钟，访问 `https://你的用户名.github.io/self-media-workbench`

### 方式四：Cloudflare Pages

1. 打开 [https://dash.cloudflare.com](https://dash.cloudflare.com) → Pages
2. 点击 Create a project → Upload assets
3. 上传本文件夹
4. 获得 `https://你的项目名.pages.dev` 链接

## 本地预览

如果只想在自己电脑上看看效果：

```bash
# 方式 A：Python
python3 -m http.server 8080

# 方式 B：Node.js
npx serve .
```

然后浏览器访问 `http://localhost:8080`

## 文件说明

- `index.html`：完整的工作台应用（单文件，包含所有 CSS 和 JS）
- `README.md`：本说明文件

## 注意事项

- 当前为前端演示版本，AI 能力由本地 Mock 数据模拟
- 后续可接入真实大模型 API，替换 `app.js` 中的生成逻辑即可
- 视频上传、历史数据导入等功能需要部署到 HTTPS 环境后体验最佳
