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
- **字体**：系统字体栈，中英文混排优化

## 样式定制

在 jekyll-now 默认主题基础上进行了全面的视觉升级：

- **设计变量系统**：通过 CSS 自定义属性定义完整的色彩、间距、阴影、圆角体系（`_sass/_variables.scss`）
- **自动暗色模式**：基于 `prefers-color-scheme` 媒体查询，无需手动切换
- **响应式布局**：640px 断点，移动端触控友好的导航和排版
- **微交互动效**：导航 hover 过渡、页面淡入动画、链接下划线偏移
- **代码高亮**：Rouge 语法高亮配色匹配整体色彩系统，亮/暗双主题
- **打印样式**：`@media print` 隐藏导航和页脚，优化排版
- **粘性头部**：`position: sticky` + `backdrop-filter` 毛玻璃效果

### 样式文件结构

```
_sass/
├── _variables.scss    # 设计变量（颜色、间距、字体、阴影、过渡）
├── _highlights.scss   # Rouge 语法高亮配色
├── _svg-icons.scss    # SVG 图标样式
└── _reset.scss        # CSS Reset（未修改）
style.scss             # 主样式入口
```

## 本地开发

需安装 Ruby 及 Jekyll：

```bash
gem install jekyll bundler
bundle install
bundle exec jekyll serve
```

或直接推送到 GitHub，由 GitHub Pages 自动构建部署。

## 许可

本项目基于 [jekyll-now](https://github.com/barryclark/jekyll-now) 的 MIT 协议。
