# Eureka

![Eureka](./assets/image.png)

> Academic paper research workflow tools

A collection of independent skills for paper search and HTML report generation.

## Skills

### eureka-paper-search

Multi-source academic paper search tool with automatic fallback.

- **Features**:
  - Search from arXiv, Semantic Scholar, DBLP
  - Automatic fallback mechanism
  - Configurable research interests
  - Generates structured notes (Obsidian/Markdown)

- **Usage**:
  ```
  /eureka-paper-search llm_agent
  /eureka-paper-search memory_skills
  /eureka-paper-search 2026-03-17 reasoning
  ```

### eureka-paper-html

Generate beautiful HTML reports from paper data.

- **Features**:
  - Minimalism & Swiss Style design
  - Responsive layout
  - Dark mode support
  - Accessibility optimized

- **Usage**:
  ```
  /eureka-paper-html --input results.json --output report.html
  /eureka-paper-html --topic llm_agent --date 2026-03-17
  ```

## Installation

Copy skills to your Claude Code skills directory:

```bash
cp -r skills/eureka-paper-search ~/.claude/skills/
cp -r skills/eureka-paper-html ~/.claude/skills/
```

## Configuration

Edit `references/preference.md` in each skill to configure:

- Research interests (keywords, topics)
- Output targets (Obsidian/Markdown/HTML)
- Data source preferences

## Design System

eureka-paper-html uses:

- **Font**: Inter (body), JetBrains Mono (code)
- **Colors**: #2563EB (primary), #3B82F6 (secondary), #F97316 (CTA)
- **Style**: Minimalism & Swiss Style

## License

MIT