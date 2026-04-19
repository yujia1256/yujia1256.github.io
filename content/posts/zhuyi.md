---
date: '2026-04-19T13:25:44+08:00'
draft: true
title: 'Zhuyi'
---
hugo new posts/zhuyi.md
这是终端新建文件的代码，
要在浏览器中看到这个页面，首先要在终端cd my_blog
进入放hugo模版的地方
这里有一个最简单的流程，让你在几分钟内看到自己的博客网页：


第一步：检查并更新
打开终端（Terminal），先确保你的工具是最新的：
brew update
brew upgrade hugo


第二步：建立你的“基地”
找一个你存放代码的文件夹，执行：
hugo new site my-awesome-blog
cd my-awesome-blog


第三步：挑一件“衣服”（安装主题）
Hugo 本身是不带皮肤的，必须装一个主题。最快的方法是直接下载一个流行的主题（比如 Ananke）：
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> hugo.toml


第四步：写下第一句话
hugo new posts/hello-world.md


这会在 content/posts 目录下生成一个 Markdown 文件。你可以用你的编辑器（比如 VS Code）打开它，在里面写点东西。
第五步：见证奇迹的时刻
输入以下命令启动本地服务器：
hugo server -D


现在，在浏览器里访问 http://localhost:1313，你就能看到你的博客已经在本地运行了！
接下来做什么？
当你写好了文章，准备让全世界看到时，通常有两种路线：
1.走 GitHub Pages 路线： 把代码推送到 GitHub，利用 GitHub Actions 自动发布（最省心，不用管服务器）。
2.走云服务器路线： 运行 hugo 命令生成静态文件，然后扔进你之前配置好的 Nginx 目录里。
