# Eureka

![Eureka](./assets/image.png)

> 学术论文研究工作流工具

独立的论文搜索和 HTML 汇报生成工具集合。

## Skills

### eureka-paper-search

多数据源论文搜索工具，支持自动回退。

- **功能**:
  - 从 arXiv、Semantic Scholar、DBLP 搜索
  - 自动回退机制
  - 可配置研究兴趣
  - 生成结构化笔记（Obsidian/Markdown）

- **用法**:
  ```
  /eureka-paper-search llm_agent
  /eureka-paper-search memory_skills
  /eureka-paper-search 2026-03-17 reasoning
  ```

### eureka-paper-html

从论文数据生成美观的 HTML 汇报。

- **功能**:
  - 极简瑞士风格设计
  - 响应式布局
  - 暗色模式支持
  - 无障碍优化

- **用法**:
  ```
  /eureka-paper-html --input results.json --output report.html
  /eureka-paper-html --topic llm_agent --date 2026-03-17
  ```

## 安装

将 skills 复制到你的 Claude Code skills 目录：

```bash
cp -r skills/eureka-paper-search ~/.claude/skills/
cp -r skills/eureka-paper-html ~/.claude/skills/
```

## 配置

编辑每个 skill 中的 `references/preference.md`：

- 研究兴趣（关键词、主题）
- 输出目标（Obsidian/Markdown/HTML）
- 数据源偏好

## 设计系统

eureka-paper-html 使用：

- **字体**: Inter（正文）、JetBrains Mono（代码）
- **配色**: #2563EB（主色）、#3B82F6（次色）、#F97316（CTA）
- **风格**: 极简瑞士风格

## 许可证

MIT