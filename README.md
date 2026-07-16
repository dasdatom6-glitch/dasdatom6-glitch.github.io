# My Tech Blog

基于 Hugo + Stack 主题的个人技术博客，部署在 GitHub Pages。

## 快速开始

### 1. 安装 Hugo

```bash
# macOS
brew install hugo

# Linux (Debian/Ubuntu)
sudo apt install hugo

# Windows
# 下载: https://github.com/gohugoio/hugo/releases
# 选择 hugo_extended_*_windows-amd64.zip
```

### 2. 克隆并初始化

```bash
# 克隆你的仓库（已包含项目文件）
git clone https://github.com/<你的用户名>/<你的用户名>.github.io.git
cd <你的用户名>.github.io

# 添加 Stack 主题
git submodule add https://github.com/CaiJimmy/hugo-theme-stack.git themes/hugo-theme-stack
```

### 3. 本地预览

```bash
hugo server -D
# 打开 http://localhost:1313
```

### 4. 写新文章

```bash
hugo new content posts/my-new-post.md
```

然后编辑 `content/posts/my-new-post.md`，把 `draft: true` 改为 `draft: false`。

### 5. 部署

推送到 GitHub 的 `main` 分支即可自动部署（已配置 GitHub Actions）：

```bash
git add .
git commit -m "new post"
git push origin main
```

几分钟后访问 `https://<你的用户名>.github.io`。

## 项目结构

```
.
├── hugo.toml              # 站点配置
├── content/
│   ├── posts/             # 博客文章
│   └── about/             # 关于页面
├── themes/
│   └── hugo-theme-stack/  # 主题（git submodule）
├── static/
│   └── img/               # 静态图片
└── .github/workflows/
    └── hugo.yml           # GitHub Actions 部署配置
```

## 自定义

- **修改标题/描述**: 编辑 `hugo.toml` 中的 `title` 和 `params.sidebar.subtitle`
- **修改头像**: 替换 `static/img/avatar.png`
- **添加页面**: 在 `content/` 下创建新目录和 `index.md`
- **修改菜单**: 编辑 `hugo.toml` 中的 `[[menu.main]]` 部分
