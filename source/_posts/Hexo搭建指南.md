---
title: 使用 Hexo 搭建个人博客完全指南
date: 2026-07-15 21:30:00
tags:
- Hexo
- 教程
- 博客
categories:
- 技术
---

# 使用 Hexo 搭建个人博客完全指南

Hexo 是一个快速、简洁且高效的博客框架，支持 Markdown 语法，可以轻松生成静态网站。

## 准备工作

### 安装 Node.js

Hexo 基于 Node.js，所以首先需要安装 Node.js 环境。

### 安装 Hexo

```bash
npm install -g hexo-cli
```

### 初始化博客

```bash
hexo init my-blog
cd my-blog
npm install
```

## 写文章

在 `source/_posts` 目录下创建 Markdown 文件即可。

```markdown
---
title: 文章标题
date: 2026-01-01 12:00:00
tags:
- 标签1
- 标签2
---

文章内容...
```

## 生成静态文件

```bash
hexo generate
```

## 部署到 Cloudflare Pages

1. 将代码推送到 GitHub
2. 在 Cloudflare Pages 中创建新项目
3. 设置构建命令：`npm install && npx hexo generate`
4. 设置输出目录：`public`

完成！你的博客就上线了。