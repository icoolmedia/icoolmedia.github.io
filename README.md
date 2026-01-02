# 刘志鹏的技术博客

> 音视频技术 · 数学之美 · 算法探索

这是一个基于 Jekyll 和 Chirpy 主题的技术博客，专为撰写包含数学公式和代码的技术文章优化。

## 🚀 快速开始（5分钟上手）

### 1. 环境要求

- macOS（已安装 Homebrew）
- Ruby 3.3（**重要：不支持 Ruby 2.x 或 4.x**）

### 2. 安装 Ruby 3.3

```bash
# 安装 Ruby 3.3
brew install ruby@3.3

# 配置环境变量
echo 'export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"' >> ~/.zshrc
echo 'export PATH="/opt/homebrew/lib/ruby/gems/3.3.0/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc

# 验证版本（应显示 3.3.x）
ruby -v
```

### 3. 安装依赖

```bash
# 进入博客目录
cd /path/to/icoolmedia.github.io

# 安装依赖（首次运行需要几分钟）
bundle install
```

### 4. 启动博客

```bash
# 方法1：使用脚本
./tools/run.sh

# 方法2：使用命令
bundle exec jekyll serve --livereload
```

### 5. 访问博客

打开浏览器访问：**http://localhost:4000**

## 📝 如何写文章

### 创建新文章

在 `_posts` 目录下创建文件，命名格式：`YYYY-MM-DD-title.md`

```bash
# 示例
touch _posts/2026-01-05-my-first-article.md
```

### 文章模板

```markdown
---
title: 你的文章标题
date: 2026-01-05 10:00:00 +0800
categories: [音视频技术, 视频编码]
tags: [H264, 算法]
math: true     # 如果有数学公式
---

## 引言

在这里开始写作...
```

### 数学公式

```markdown
行内公式：$E = mc^2$

块级公式：
$$
F(\omega) = \int_{-\infty}^{\infty} f(t)e^{-j\omega t}dt
$$
```

### 代码高亮

````markdown
```python
def hello():
    print("Hello, World!")
```
````

## 📚 详细教程

启动博客后，访问首页置顶文章：

**《Jekyll博客使用指南：从零开始写作你的技术博客》**

这篇文章包含：
- ✅ 完整的环境搭建指南（含所有踩过的坑）
- ✅ 详细的写作技巧
- ✅ 13+ 个常见问题解答
- ✅ Git 和 GitHub Pages 部署教程

## ⚠️ 常见问题速查

### Q: `bundle install` 报错版本不兼容？

**原因**：Ruby 版本不对（系统自带的 2.6.x 太旧，或 4.0.x 太新）

**解决**：
```bash
brew install ruby@3.3
echo 'export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"' >> ~/.zshrc
echo 'export PATH="/opt/homebrew/lib/ruby/gems/3.3.0/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
bundle install
```

### Q: 新文章不显示？

**检查**：
1. 文件名格式：`YYYY-MM-DD-title.md`
2. 日期不是未来
3. Front Matter 格式正确

### Q: 图片在 VSCode 中看不到？

**这是正常的！** VSCode Markdown 预览不支持绝对路径。启动博客在浏览器中预览。

### Q: 更多问题？

查看博客中的完整教程文章，有详细的问题解答和解决方案。

## 📂 目录结构

```
.
├── _config.yml              # 博客配置
├── _posts/                  # 📝 所有文章
├── _tabs/about.md           # 关于页面
├── assets/img/              # 🖼️ 图片文件夹
│   └── lzp.jpg              # 头像（需要你添加）
└── tools/run.sh             # 启动脚本
```

## 🎯 下一步

1. ✅ 添加头像：将 `lzp.jpg` 放到 `assets/img/` 目录
2. ✅ 阅读教程：访问博客首页的置顶文章
3. ✅ 写第一篇：创建你的第一篇技术文章
4. ✅ 发布部署：推送到 GitHub Pages

## 📖 相关文档

- [Jekyll 官方文档](https://jekyllrb.com/docs/)
- [Chirpy 主题文档](https://chirpy.cotes.page/)
- [Markdown 语法指南](https://www.markdownguide.org/)

---

💡 **提示**：遇到任何问题，先查看博客中的完整教程文章！所有踩过的坑都记录在里面了。
