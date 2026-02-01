# 如何启用 GitHub Pages

本仓库已经配置好了 GitHub Pages 博客所需的所有文件。按照以下步骤启用你的个人博客：

## 步骤 1: 进入仓库设置

1. 在 GitHub 仓库页面，点击顶部的 **Settings**（设置）标签
2. 在左侧菜单中找到并点击 **Pages**

## 步骤 2: 配置 GitHub Pages

1. 在 "Source" 部分，选择你想要部署的分支：
   - 选择 `copilot/add-personal-blog-using-github-pages` 分支（当前分支）
   - 或者将更改合并到 `main` 分支后选择 `main` 分支
2. 确保根目录选择为 `/ (root)`
3. 点击 **Save** 按钮

## 步骤 3: 等待部署

1. GitHub 会自动开始构建你的网站
2. 部署通常需要 1-5 分钟
3. 完成后，你会看到一个绿色的成功消息和网站 URL

## 步骤 4: 访问你的博客

你的博客将会在以下地址可访问：

```
https://walter1026.github.io/skills-introduction-to-github/
```

## 博客结构

- `_config.yml` - Jekyll 配置文件，包含网站标题、描述等设置
- `index.md` - 博客首页
- `about.md` - 关于页面
- `_posts/` - 博客文章目录
  - `2026-02-01-welcome.md` - 示例博客文章

## 如何添加新文章

要添加新的博客文章：

1. 在 `_posts/` 目录下创建新文件
2. 文件名格式：`YYYY-MM-DD-title.md`（例如：`2026-02-01-my-post.md`）
3. 文件开头需要包含 YAML front matter：

```markdown
---
layout: post
title: "你的文章标题"
date: 2026-02-01 12:00:00 +0800
categories: blog
tags: [标签1, 标签2]
---

你的文章内容...
```

4. 使用 Markdown 格式编写内容
5. 提交并推送到 GitHub，网站会自动更新

## 自定义博客

### 修改网站信息

编辑 `_config.yml` 文件来修改：
- 网站标题和描述
- 作者信息
- 主题设置

### 更换主题

GitHub Pages 支持多种主题。在 `_config.yml` 中修改 `theme` 字段：

```yaml
theme: minima  # 或其他支持的主题
```

支持的主题列表：https://pages.github.com/themes/

## 问题排查

如果网站无法访问：

1. 检查 GitHub Pages 设置是否正确保存
2. 等待几分钟让部署完成
3. 检查仓库的 Actions 标签页，查看构建状态
4. 确保 `_config.yml` 文件没有语法错误

## 更多资源

- [GitHub Pages 文档](https://docs.github.com/pages)
- [Jekyll 文档](https://jekyllrb.com/docs/)
- [Markdown 语法](https://www.markdownguide.org/)

祝你使用愉快！🎉
