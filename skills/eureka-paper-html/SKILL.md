---
name: eureka-paper-html
description: Generate beautiful HTML reports from paper data. Uses Minimalism & Swiss Style design system with responsive layout and dark mode support. Perfect for paper presentations and sharing.
---

# Skill: eureka-paper-html

> HTML Paper Report Generation

## Overview

eureka-paper-html generates beautiful HTML reports from paper data using professional design systems. Suitable for paper presentations, sharing, and display.

## Design System

Uses **Minimalism & Swiss Style**:
- **Fonts**: Inter (sans-serif), JetBrains Mono (code)
- **Colors**: #2563EB (primary), #3B82F6 (secondary), #F97316 (CTA)
- **Features**: Clean, clear, high-contrast, responsive

## Usage

### Basic Usage

```
/eureka-paper-html --input results.json --output report.html
```

### Specify Topic and Date

```
/eureka-paper-html --topic llm_agent --date 2026-03-17
```

### Full Parameters

```
/eureka-paper-html \
  --input results.json \
  --output report.html \
  --topic llm_agent \
  --date 2026-03-17 \
  --title "LLM Agent Research Progress"
```

## Input Format

Accepts JSON format paper data:

```json
[
  {
    "id": "2603.12933",
    "title": "Paper Title",
    "authors": ["Author1", "Author2"],
    "abstract": "Paper abstract...",
    "published": "2026-03-13",
    "source": "arXiv"
  }
]
```

## Output

Generates HTML file containing:
- Header (date, title)
- Overview section (trends, hotspots)
- Paper card list
- PDF/arXiv links
- Responsive layout

## Design Features

1. **Card-based layout**: Each paper as independent card
2. **Responsive**: Adapts to mobile, tablet, desktop
3. **Dark mode**: Auto-adapts to system theme
4. **Accessibility**: Supports reduced-motion
5. **Fast loading**: Lightweight CSS

## Dependencies

- Python 3.x
- No extra dependencies (pure CSS)

## Relationship with eureka-paper-search

eureka-paper-html is a standalone skill, can be used independently:

- **Standalone**: Have paper data → Generate HTML
- **Combined**: eureka-paper-search → eureka-paper-html

```bash
# Combined usage example
eureka-paper-search llm_agent --output results.json
eureka-paper-html --input results.json --output report.html
```