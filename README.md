<h1 align="center">hexo-editor</h1>

<p align="center">
  <img src="https://img.shields.io/github/languages/code-size/MaLuns/hexo-editor?logo=Visual Studio Code&logoColor=blue" alt="GitHub code size in bytes">
  <a title="GitHub Discussions" target="_blank" href="https://github.com/MaLuns/hexo-editor/discussions">
    <img src="https://img.shields.io/github/discussions/MaLuns/hexo-editor?color=9cf&logo=github" alt="GitHub Discussions">
  </a>
  <a title="SATA License" target="_blank" href="https://github.com/zTrix/sata-license">
    <img src="https://img.shields.io/badge/license-SATA-green.svg" alt="SATA License">
  </a>
</p>

<div align="center">
    在线 Hexo 写作编辑器。
</div>

## 截图 | Screenshots

<p align="center">
  <img width="80%" style="border-radius:8px;" src="public/demo.png" alt="demo.png" border="0" />
</p>

## 功能 | Feature

- [x] 文章增删改和预览
- [x] 发布草稿、下架发布
- [x] Markdown 编辑、预览、格式化
- [x] front-matters 编辑
- [x] 图片粘贴、Markdown 语法提示、解析 HTML
- [x] 主题切换
- [x] 静态资源管理
- [x] 命令面板
- [ ] 搜索文章内容
- [ ] 支持图床
- [ ] Markdown 同步滚动
- [ ] 使用 Github 仓库
- [ ] 更多

## 部署到 GitHub Pages | Deploy to GitHub Pages

### 方法一：使用 GitHub Actions（推荐）

1. Fork 这个仓库到您的 GitHub 账户
2. 在您的仓库设置中启用 GitHub Pages：
   - 进入 Settings → Pages
   - Source 选择 "GitHub Actions"
3. 推送代码到 master 分支，GitHub Actions 会自动构建并部署
4. 访问 `https://yourusername.github.io/hexo-editor/`

### 方法二：手动部署

```bash
# 克隆项目
git clone https://github.com/yourusername/hexo-editor.git
cd hexo-editor

# 安装依赖
npm install

# 构建项目
npm run build

# 部署到 gh-pages 分支
npm install -g gh-pages
gh-pages -d dist
```

## 贡献 | Contribute

欢迎各种各样的 PR（魔改也是可以的！）

All kinds of PR are welcomed, including crazy change!

如果这项目帮到你了，点个爱的五角星呗~

If this project helped you a bit, please leave a ⭐ with your ❤ :p!
