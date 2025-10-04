# GitHub Pages 部署指南

## 快速部署步骤

### 1. Fork 项目
- 访问 [hexo-editor](https://github.com/MaLuns/hexo-editor)
- 点击右上角的 "Fork" 按钮
- 将项目 fork 到您的 GitHub 账户

### 2. 配置 GitHub Pages
1. 进入您 fork 的仓库
2. 点击 "Settings" 标签页
3. 在左侧菜单中找到 "Pages"
4. 在 "Source" 部分选择 "GitHub Actions"
5. 保存设置

### 3. 推送代码
```bash
# 克隆您的 fork
git clone https://github.com/yourusername/hexo-editor.git
cd hexo-editor

# 推送代码到 master 分支
git push origin master
```

### 4. 自动部署
- GitHub Actions 会自动检测到代码推送
- 自动构建项目并部署到 GitHub Pages
- 部署完成后，访问 `https://yourusername.github.io/hexo-editor/`

## 部署配置说明

### 子路径部署
项目已配置为子路径部署，访问地址为：
```
https://yourusername.github.io/hexo-editor/
```

### 根路径部署
如果您想部署到根路径（替换现有 GitHub Pages），需要修改 `vite.config.ts`：

```typescript
export default defineConfig({
  base: '/', // 改为根路径
  // ... 其他配置
});
```

## 故障排除

### 构建失败
如果 GitHub Actions 构建失败：
1. 检查 Node.js 版本兼容性
2. 确保所有依赖都已正确安装
3. 查看 Actions 日志获取详细错误信息

### 页面无法访问
1. 确认 GitHub Pages 已启用
2. 检查仓库设置中的 Pages 配置
3. 等待几分钟让 DNS 生效

## 自定义配置

### 修改项目名称
1. 修改 `package.json` 中的 `name` 字段
2. 修改 `vite.config.ts` 中的 `base` 路径
3. 更新 README.md 中的链接

### 添加自定义域名
1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容为您的域名（如：`example.com`）
3. 在 DNS 设置中添加 CNAME 记录指向 `yourusername.github.io`
