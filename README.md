# 冉起阳 · 个人展示平台

一个使用原生 HTML、CSS 和 JavaScript 构建的个人主页，用于介绍我的学习经历、嵌入式与自动控制项目、技能和荣誉。

## 页面内容

- 个人介绍与联系方式
- 已完成项目展示，支持按嵌入式控制、硬件/PCB 和团队/竞赛分类筛选，并可查看项目详情
- 未来及进行中的项目
- 技能、教育经历和荣誉证书
- 移动端导航、滚动显示动画和项目详情弹窗

## 在线预览

GitHub 仓库：[Huluobo-dev/turbo-octo-invention](https://github.com/Huluobo-dev/turbo-octo-invention)

如已启用 GitHub Pages，可通过仓库 **Settings → Pages** 中显示的网址访问网页。

## 本地运行

本项目是静态网页，无需安装依赖或构建工具。克隆仓库后，在浏览器中打开 `index.html` 即可预览。也可以使用任意本地静态 HTTP 服务器提供项目目录。

```bash
git clone https://github.com/Huluobo-dev/turbo-octo-invention.git
cd turbo-octo-invention
```

## 项目结构

```text
.
├── index.html       # 页面结构与内容
├── styles.css       # 页面样式与响应式布局
├── script.js        # 项目、技能、经历和荣誉数据及交互
├── assets/
│   └── avatar.jpg   # 个人头像
└── resume_text.txt  # 简历文本资料
```

## 更新展示内容

在 `script.js` 中编辑对应的数据数组，页面会自动生成相应内容：

- `projects`：已完成项目
- `futureProjects`：规划中或进行中的项目，`status` 可设为 `plan` 或 `doing`
- `skills` 与 `skillTags`：技能条和技能标签
- `timeline`：教育及经历
- `awards`：荣誉与证书

修改个人照片时，替换 `assets/avatar.jpg`，并保持文件名不变；若使用其他文件名，请同步修改 `index.html` 中头像的图片路径。

## 使用技术

- HTML5
- CSS3
- 原生 JavaScript
