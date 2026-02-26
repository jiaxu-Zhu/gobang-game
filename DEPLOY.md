# GitHub Pages 部署指南

## 步骤 1: 创建 GitHub 仓库

1. 访问 https://github.com/new
2. 仓库名称建议：`gobang-game` 或 `五子棋`
3. 选择 **Public**（公开仓库，免费使用GitHub Pages）
4. **不要**勾选 "Initialize this repository with a README"
5. 点击 "Create repository"

## 步骤 2: 推送代码到 GitHub

在您的本地电脑上执行以下命令（假设您已安装git）：

```bash
# 克隆这个文件夹到本地（或者直接复制文件）
# 如果您有文件，可以直接在GitHub网页上传

# 方法A：通过Git命令行
cd /path/to/gobang-folder
git remote add origin https://github.com/您的用户名/gobang-game.git
git branch -M main
git push -u origin main
```

**方法B：通过GitHub网页直接上传**
1. 进入刚创建的仓库页面
2. 点击 "upload an existing file"
3. 拖拽整个 `gobang` 文件夹内容上传
4. 点击 "Commit changes"

## 步骤 3: 启用 GitHub Pages

1. 进入仓库的 **Settings** 标签页
2. 左侧菜单点击 **Pages**
3. 在 "Build and deployment" 部分：
   - Source: 选择 **Deploy from a branch**
   - Branch: 选择 `main` 分支，文件夹选择 `/ (root)`
4. 点击 **Save**

## 步骤 4: 访问您的游戏

等待1-2分钟后，访问：

```
https://您的用户名.github.io/gobang-game/
```

即可开始游戏！

## 注意事项

- 首次部署可能需要几分钟
- 如果404，请稍等片刻后刷新
- 每次更新代码后，GitHub Pages会自动重新部署

## 备用方案

如果GitHub Pages无法访问，也可以考虑：
- **Vercel**: https://vercel.com (导入GitHub仓库即可)
- **Netlify**: https://netlify.com (拖拽文件夹即可部署)
- **Cloudflare Pages**: https://pages.cloudflare.com

这些平台都提供免费的静态网站托管。