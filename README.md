# 沈和巧的个人博客项目

## 📝 项目简介

这是沈和巧（学号：202215008363）为《云计算原理与应用》课程期末作业搭建的个人博客项目。博客基于Hexo静态博客框架构建，采用Butterfly主题，主要记录数据科学、云计算及相关技术的学习笔记与实践经验。

## 🏫 课程信息

- **课程名称**：《云计算原理与应用》
- **学期**：2025-2026学年第一学期
- **专业班级**：2022级数据科学与大数据技术本科（数字平台运维方向）
- **学生姓名**：沈和巧
- **学号**：202215008363
- **项目名称**：shenheqiao-blog

## 🔗 访问地址

### 在线访问
- **GitHub Pages主站**：[https://wdwsaa.github.io/](https://wdwsaa.github.io/)
- **备用访问地址**：[https://wdwsaa.github.io/shenheqiao-blog/](https://wdwsaa.github.io/shenheqiao-blog/)

### 本地开发访问
- **本地预览地址**：http://localhost:4000

## 🚀 快速开始

### 环境要求
- Node.js（v14.0或更高版本）
- Git
- npm（Node.js包管理器）

### 本地运行步骤

#### 1. 克隆项目
```bash
git clone https://github.com/wdwsaa/wdwsaa.github.io.git
cd wdwsaa.github.io
```

#### 2. 安装依赖
```bash
npm install
```

#### 3. 启动本地服务器
```bash
# 清理缓存并生成静态文件
hexo clean && hexo generate

# 启动本地服务器
hexo server

# 打开浏览器访问 http://localhost:4000
```

#### 4. 创建新文章
```bash
# 创建一篇新文章
hexo new "文章标题"

# 编辑文章内容（Markdown格式）
# 文件位于：source/_posts/文章标题.md
```

## 📦 项目部署

### 自动部署到GitHub Pages
```bash
# 一键部署（清理、生成、部署）
hexo clean && hexo generate && hexo deploy
```

### 部署验证
1. 访问 [https://wdwsaa.github.io/](https://wdwsaa.github.io/)
2. 等待1-2分钟让GitHub Pages生效
3. 按 `Ctrl + F5` 强制刷新浏览器缓存

## 📁 项目结构

```
shenheqiao-blog/
├── _config.yml          # Hexo主配置文件
├── package.json         # 项目依赖配置
├── package-lock.json    # 依赖锁定文件
├── scaffolds/           # 文章模板目录
├── source/              # 源文件目录
│   ├── _posts/         # 文章目录（所有博文.md文件）
│   ├── about/          # "关于"页面
│   ├── categories/     # 分类页面
│   └── tags/           # 标签页面
├── themes/              # 主题目录
│   └── butterfly/      # Butterfly主题文件
├── public/              # 生成的静态文件（部署后生成）
└── README.md           # 项目说明文件（本文件）
```

## ⚙️ 配置文件说明

### 博客基本配置（_config.yml）
```yaml
# 站点信息
title: 沈和巧的博客
subtitle: 云计算与数据科学学习笔记
description: 这是我的个人博客，创建于12:48
keywords: 云计算, 数据科学, 大数据, 技术博客
author: 202215008363
language: zh-CN

# 主题配置
theme: butterfly

# 部署配置
deploy:
  type: git
  repo: git@github.com:wdwsaa/wdwsaa.github.io.git
  branch: main
```

### 文章Front-matter格式
```yaml
---
title: 文章标题
date: 2025-01-15 14:30:00
tags:
  - 标签1
  - 标签2
categories: 分类名称
cover: https://images.unsplash.com/图片地址
description: 文章简要描述
---
```

## 🛠️ 常用命令

| 命令 | 说明 | 简写 |
|------|------|------|
| `hexo new "文章标题"` | 创建新文章 | `hexo n` |
| `hexo generate` | 生成静态文件 | `hexo g` |
| `hexo server` | 启动本地服务器 | `hexo s` |
| `hexo deploy` | 部署到GitHub | `hexo d` |
| `hexo clean` | 清理缓存文件 | - |
| `hexo clean && hexo g && hexo d` | 一键清理、生成、部署 | - |

## 🎨 主题定制

本项目使用Butterfly主题，可以通过以下方式定制：

1. **修改主题配置**：编辑 `_config.yml` 中的主题相关设置
2. **自定义样式**：在 `source/css/custom.css` 中添加CSS样式
3. **修改布局**：编辑 `themes/butterfly/layout/` 下的模板文件

## ❓ 常见问题

### 1. 本地无法启动服务器
```bash
# 检查端口是否被占用
hexo server -p 5000

# 检查依赖是否完整
npm install
```

### 2. 部署失败
- 检查Git配置：`git config --global user.name` 和 `git config --global user.email`
- 验证SSH密钥：`ssh -T git@github.com`
- 检查部署配置中的仓库地址和分支

### 3. 文章不显示
- 检查文章日期是否为未来时间
- 在 `_config.yml` 中设置 `future: true` 以显示未来文章
- 检查Front-matter格式是否正确

### 4. 页面样式异常
```bash
# 重新安装主题
npm install hexo-theme-butterfly --save

# 清理缓存重新生成
hexo clean && hexo generate
```

## 📊 项目状态

- ✅ 博客框架搭建完成
- ✅ 主题定制完成
- ✅ 自动化部署配置完成
- ✅ 基础内容建设完成
- ✅ GitHub Pages正常访问

## 📞 联系信息

- **学生**：沈和巧
- **学号**：202215008363
- **GitHub账号**：[wdwsaa](https://github.com/wdwsaa)
- **项目仓库**：[https://github.com/wdwsaa/wdwsaa.github.io](https://github.com/wdwsaa/wdwsaa.github.io)

## 📄 许可证

本项目采用 MIT 许可证。

---

**最后更新**：2025年1月  
**项目状态**：正常运行中

> **提示**：本项目是《云计算原理与应用》课程期末作业，展示了静态博客搭建、主题定制、自动化部署等云计算相关技能。
