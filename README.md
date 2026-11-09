# 李屹然 · 个人主页

基于 [Academic Pages](https://github.com/academicpages/academicpages.github.io) 和 Jekyll。网站展示软件工程背景、两个项目及公开版履历。

[访问个人主页](https://xiaoranxiaoran.github.io/)

## 修改内容

| 内容 | 文件 |
| --- | --- |
| 首页介绍与关注方向 | `_pages/about.md` |
| 教育背景、技能与荣誉 | `_pages/cv.md` |
| 项目介绍、技术栈、展示顺序 | `_portfolio/` |
| 顶部导航 | `_data/navigation.yml` |
| 站点名称、可公开的邮箱 | `_config.yml` |
| 主页样式 | `assets/css/profile.css` |

如需公开邮箱，可填写 `_config.yml` 中的 `author.email`。站点地址与 GitHub 账号由部署工作流根据仓库自动填写。

## 发布更新

编辑文件并提交到 `main` 后，GitHub Actions 会自动构建和部署。构建状态可在仓库的 **Actions → Deploy personal site to GitHub Pages** 中查看。

## 本地预览

准备 Node.js 和带编译工具的 Ruby 3.3 环境。Windows 可使用 RubyInstaller + Devkit。

```powershell
bundle install
npm install --no-package-lock
npm run build:js
bundle exec jekyll serve
```

打开 [http://localhost:4000](http://localhost:4000) 预览。模板采用 MIT 许可，详见 `LICENSE`。
