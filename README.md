# nexipher.github.io

贺杰（Jie He）的个人学术主页，托管于 GitHub Pages，基于 [jekyll-now](https://github.com/barryclark/jekyll-now) 构建。

## 页面

| 页面 | 路径 | 说明 |
| --- | --- | --- |
| 首页 | `/` | 个人简介、教育背景、科研经历、荣誉奖项 |
| About | `/about` | 详细信息 |
| Thanks | `/thanks` | 致谢 |

## 技术栈

- **静态站点生成器**：Jekyll（GitHub Pages 自动构建）
- **模板引擎**：Liquid
- **样式预处理**：SCSS（`_sass/` 目录，模块化 partials）
- **代码高亮**：Rouge
- **字体**：宋体风格标题搭配系统无衬线正文，中英文混排优化，无外部字体请求

## 样式定制

在 jekyll-now 默认主题基础上进行了全面的视觉升级：

- **设计变量系统**：通过 CSS 自定义属性定义完整的色彩、间距、阴影、圆角体系（`_sass/_variables.scss`）
- **自动暗色模式**：基于 `prefers-color-scheme` 媒体查询，无需手动切换
- **响应式布局**：电脑端个人信息侧栏与正文双栏，760px 以下切换为纵向布局
- **内容层级**：放大头像、页内目录、成绩对照表、项目职责与带日期的奖项列表
- **交互细节**：当前页面导航提示、键盘焦点、跳转正文、减少动态效果偏好
- **代码高亮**：Rouge 语法高亮配色匹配整体色彩系统，亮/暗双主题
- **打印样式**：`@media print` 隐藏导航和页脚，优化排版
- **阅读体验**：电脑端侧栏随滚动保持可见，正文无入场动画，标题采用宋体风格字体栈

### 样式文件结构

```
_sass/
├── _variables.scss    # 设计变量（颜色、间距、字体、阴影、过渡）
├── _base.scss         # 基础排版、链接、键盘访问
├── _layout.scss       # 个人信息侧栏、导航、正文、页脚
├── _components.scss   # 简介、成绩表、项目、奖项与技能列表
├── _animations.scss   # 减少动态效果偏好
├── _mobile.scss       # 移动端适配
├── _print.scss        # 打印样式
├── _highlights.scss   # Rouge 语法高亮配色
└── _reset.scss        # CSS Reset（未修改）
style.scss             # 主样式入口
```

## 本地开发

需安装 Ruby 及 Bundler，仓库中的 `Gemfile` 使用 GitHub Pages 依赖集：

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

或直接推送到 GitHub，由 GitHub Pages 自动构建部署。

`_config.yml` 中的 `url` 为正式站点地址；若部署到子目录，需相应设置 `baseurl`。页面和资源链接会自动使用该前缀。

## 许可

感谢 barryclark 开发的 [jekyll-now](https://github.com/barryclark/jekyll-now) 项目，简化了 Jekyll + GitHub Pages 的部署流程，让个人主页搭建变得零门槛。
