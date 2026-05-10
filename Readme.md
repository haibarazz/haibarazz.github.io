# haibarazz.github.io

这是 `https://haibarazz.github.io/` 的 GitHub Pages 个人主页仓库。

## 维护方式

主页入口是 `index.html`，样式在 `assets/css/site.css`，个人信息在
`_data/profile.yml`，项目列表在 `_data/projects.yml`。

这个仓库依赖 GitHub Pages 云端 Jekyll 渲染。本地不需要安装 Jekyll、Node
构建工具或其他依赖；push 到 `main` 后 GitHub 会自动生成线上页面。

后续新增项目时，优先只改 `_data/projects.yml`：

```yaml
- slug: "new-project"
  order: 7
  title: "New Project"
  role: "AI tool"
  category_id: "agent"
  category_label: "Agent 研究"
  status: "Active"
  visibility: "Public"
  year: "2026"
  repo: "https://github.com/haibarazz/new-project"
  demo: ""
  featured: false
  summary: "一句话说明项目解决什么问题。"
  impact: "说明技术亮点、可验证结果或当前进度。"
  tags:
    - "Python"
    - "LLM"
  highlights:
    - "亮点 1"
    - "亮点 2"
```

只要 push 到 `main`，GitHub Pages 会自动更新线上页面。
