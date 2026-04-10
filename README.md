# 我的 Jekyll 个人主页
基于 [jekyll-now](https://github.com/barryclark/jekyll-now) 开源项目搭建的个人主页，无需本地编译环境，直接通过 GitHub Pages 即可快速部署轻量、美观的静态个人主页。

## 🌟 项目特点
- 零本地配置：无需安装 Ruby、Jekyll 等依赖，所有修改直接通过 GitHub 网页端完成
- 快速部署：提交代码后 GitHub Pages 自动构建，几分钟内即可上线
- 极简定制：仅需修改少量配置文件，即可自定义个人信息、主题样式
- 内置功能：支持博客发布、Markdown 渲染、代码高亮、响应式布局

## 🚀 快速上手（基于我的搭建流程）
### 1. 复刻仓库
- 访问 [jekyll-now 仓库](https://github.com/barryclark/jekyll-now)，点击 `Use this template` 复刻到自己的 GitHub 账号
- 仓库命名规则：`你的用户名.github.io`（GitHub Pages 自动识别该命名并部署）

### 2. 访问个人主页
提交修改后，等待 1-2 分钟，访问 `https://你的用户名.github.io` 即可看到你的个人主页。

## 🎨 自定义修改
### 更换主题样式
- 修改 `css/main.scss` 文件，自定义颜色、字体、布局等样式
- 或直接替换 `_layouts` 目录下的模板文件，调整页面结构

### 添加/修改页面
- 根目录下添加{content}.md文件，添加自定义页面
- 在 {default.html}的 <body> 中添加导航栏链接，关联新页面

### 扩展功能（正在研究）
- 支持添加评论功能（Disqus/Giscus）{insert\_element\_3\_77ya5ZyoIGBfY29uZmlnLnk=}ml` 中配置对应参数
- 支持添加访问统计（Google Analytics/不蒜子）：在 `_includes/footer.html` 中嵌入统计代码

## 📝 我的修改记录
（可根据自己的实际修改内容补充）
1. 替换了默认头像和个人简介
3. 添加了「关于我」页面，补充个人技能和经历

## ❓ 常见问题
### 提交修改后页面没更新？
- 检查仓库命名是否符合 `用户名.github.io` 规则
- 进入仓库的 `Settings > Pages`，确认部署源为 `main` 分支，且构建状态为成功
- 清除浏览器缓存，或等待 5-10 分钟（GitHub Pages 部署可能有延迟）

## 📄 开源协议
- 本项目基于 jekyll-now 的 MIT 协议开源，你可自由修改、分发，保留原作者版权声明即可。

## 🙏 致谢
- 感谢 barryclark 开发的 jekyll-now 项目，简化了 Jekyll + GitHub Pages 的部署流程，让个人主页搭建变得零门槛。