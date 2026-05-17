# AI 小白成长之路学习进度网页

这是一个可直接部署到 GitHub Pages 的静态网页，用来在手机上查看 AI 学习路线、管理任务完成情况、记录每日学习时长，并备份/恢复学习进度。

## 文件说明

- `index.html`：网页入口，上传到 GitHub Pages 后会自动作为首页。
- `AI小白到专家学习手册.md`：完整学习手册。
- `法考学习进度.html`：参考文件，保留不修改，默认不上传到 GitHub。

## 功能

- 首页：总体进度、当前阶段、下一步任务、阶段总览。
- 路线：按阶段筛选、搜索任务、标记完成/取消完成。
- 今日：记录学习分钟数、今日笔记、一键完成下一项任务。
- 资源：集中打开课程、视频、官方文档。
- 设置：修改每周目标、导出/导入进度、重置数据。

## 数据保存

网页是纯静态页面，没有服务器和数据库。学习进度保存在当前浏览器的 `localStorage` 中。

跨设备使用时：

1. 在旧设备打开网页，进入“设置”，点击“导出”。
2. 把导出的 JSON 文件传到新设备。
3. 在新设备打开网页，进入“设置”，点击“导入”。

## 上传到 GitHub Pages

### 方法一：网页操作

1. 打开 [GitHub](https://github.com/) 并登录。
2. 点击右上角 `+`，选择 `New repository`。
3. Repository name 填：`ai-study-roadmap`。
4. 选择 `Public`。
5. 点击 `Create repository`。
6. 点击 `uploading an existing file`。
7. 上传本文件夹里的 `index.html`、`README.md`、`.gitignore`、`AI小白到专家学习手册.md`。
8. 点击 `Commit changes`。
9. 进入仓库 `Settings`。
10. 左侧选择 `Pages`。
11. Source 选择 `Deploy from a branch`。
12. Branch 选择 `main` 和 `/root`，点击 `Save`。
13. 等待 1-3 分钟，GitHub 会生成访问链接。

### 方法二：命令行

把下面的 `你的用户名` 替换成你的 GitHub 用户名：

```bash
git init
git add index.html README.md .gitignore "AI小白到专家学习手册.md"
git commit -m "Add AI study roadmap page"
git branch -M main
git remote add origin https://github.com/你的用户名/ai-study-roadmap.git
git push -u origin main
```

然后到 GitHub 仓库的 `Settings -> Pages` 启用 Pages。
