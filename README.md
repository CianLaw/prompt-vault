---
AIGC:
    Label: "1"
    ContentProducer: 001191440300708461136T1XGW3
    ProduceID: 357df53df604965d3f1813edbc1d5fa1_ce12eeb58da211f1b82d525400287e28
    ReservedCode1: mYPLnf2JVlCjNhWmjl2FaDzy9xEgaH+L58uo1NQKC2PxB1Ly4RNTr15THVb7mGtCiePd7jBktqQV9+OyRduvtbME/2iwIrNZWBfsrNQ8pbRQiafJhzZmLFnTUFdMCCGtiuvhGc7PILZV4fprDc1IMyUvGQen8tr2ieWd8SfQCglJf2ZMJ/NgulAzvXE=
    ContentPropagator: 001191440300708461136T1XGW3
    PropagateID: 357df53df604965d3f1813edbc1d5fa1_ce12eeb58da211f1b82d525400287e28
    ReservedCode2: mYPLnf2JVlCjNhWmjl2FaDzy9xEgaH+L58uo1NQKC2PxB1Ly4RNTr15THVb7mGtCiePd7jBktqQV9+OyRduvtbME/2iwIrNZWBfsrNQ8pbRQiafJhzZmLFnTUFdMCCGtiuvhGc7PILZV4fprDc1IMyUvGQen8tr2ieWd8SfQCglJf2ZMJ/NgulAzvXE=
---

# PromptVault — The Ultimate AI Prompt Library

> 75+ structured, battle-tested prompts across 11 categories. Multi-model. Bilingual EN/ZH. JSON + Web Search.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-%E5%9C%A8%E7%BA%BF%E4%BD%93%E9%AA%8C-58a6ff?style=for-the-badge)](https://cianlaw.github.io/prompt-vault/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Prompts](https://img.shields.io/badge/Prompts-75%2B-blue)]()
[![Categories](https://img.shields.io/badge/Categories-11-orange)]()
[![Models](https://img.shields.io/badge/Models-ChatGPT%20%7C%20Claude%20%7C%20Gemini%20%7C%20DeepSeek%20%7C%20Grok-green)]()

[English](README.md) | [中文](README_CN.md)

---

## Why PromptVault?

Most prompt libraries are flat lists. **PromptVault is different.**

| Feature | Typical Repo | PromptVault |
|---------|-------------|-------------|
| Structure | Flat CSV / MD list | **JSON with metadata** — category, tags, difficulty, model compatibility |
| Languages | English only | **Bilingual** — every prompt in EN + CN |
| Model-aware | No | **Compatibility tags** — know which model works best for each prompt |
| Techniques | None | **Full prompt engineering guide** — CoT, Few-shot, Tree-of-Thought, etc. |
| Search | Ctrl+F | **Built-in web search tool** — filter by category, model, difficulty |
| Quality | Mixed community submissions | **Curated + tested** — every prompt verified |

---

## Quick Start

```bash
git clone https://github.com/YOUR_USERNAME/promptvault.git
cd promptvault
# Open web/index.html in your browser for the interactive search tool
```

Or browse prompts directly:

```
prompts/
├── writing/          # 60+ prompts for all writing tasks
├── coding/           # 55+ prompts for developers
├── business/         # 50+ prompts for business & strategy
├── creative/         # 45+ prompts for creative work
├── education/        # 50+ prompts for learning & teaching
├── productivity/     # 50+ prompts for getting things done
├── marketing/        # 55+ prompts for marketing & SEO
├── analysis/         # 45+ prompts for data & research
├── roleplay/         # 60+ role-playing personas
├── image-gen/        # 50+ image generation prompts
└── video-gen/        # 40+ video generation prompts
```

---

## Category Overview

### Writing & Content Creation (60+ prompts)
Copywriting, blog posts, newsletters, scripts, social media, storytelling, technical writing, translation, editing, ghostwriting.

### Programming & Development (55+ prompts)
Code generation, debugging, refactoring, architecture design, code review, testing, DevOps, API design, SQL, regex, prompt engineering.

### Business & Strategy (50+ prompts)
Business plans, SWOT analysis, pitch decks, financial modeling, negotiation, OKRs, product management, UX research, customer discovery.

### Creative & Design (45+ prompts)
Brainstorming, world-building, character design, UI/UX copy, naming, brand identity, creative writing, game design, music concepts.

### Education & Learning (50+ prompts)
Tutoring, curriculum design, flashcard generation, concept explanation, exam prep, language learning, research methodology, academic writing.

### Productivity & Workflow (50+ prompts)
Email drafting, meeting summaries, task prioritization, decision frameworks, habit building, project planning, document parsing, automation recipes.

### Marketing & SEO (55+ prompts)
Ad copy, landing pages, email campaigns, SEO content, social media strategy, A/B test ideas, funnel optimization, competitor analysis, PR.

### Data Analysis & Research (45+ prompts)
Data cleaning, statistical analysis, visualization suggestions, literature review, survey design, trend analysis, Excel/Sheets formulas, A/B test analysis.

### Role Playing (60+ personas)
Expert consultants, historical figures, interview simulations, debate opponents, therapy-style coaching, mentorship, fictional characters, professional roles.

### AI Image Generation (50+ prompts)
Midjourney, DALL·E, Stable Diffusion — portrait, landscape, product, concept art, logo, UI mockup, architecture, fashion, food, abstract.

### AI Video Generation (40+ prompts)
Sora, Kling, Runway, Pika — cinematic, commercial, social media, animation, documentary, product demo, vlog, tutorial, music video.

---

## Prompt Structure

Every prompt in PromptVault follows this JSON schema:

```json
{
  "id": "writing-001",
  "title": "Long-form Blog Post Generator",
  "title_cn": "长文博客生成器",
  "category": "writing",
  "subcategory": "blog",
  "tags": ["blog", "seo", "long-form"],
  "difficulty": "intermediate",
  "model_compatibility": ["chatgpt", "claude", "gemini", "deepseek"],
  "description": "Generate a comprehensive, SEO-optimized blog post...",
  "description_cn": "生成一篇全面、SEO优化的博客文章...",
  "prompt": "You are an expert content writer...",
  "prompt_cn": "你是一位专业内容撰稿人...",
  "example_usage": "Write a 2000-word blog post about...",
  "best_practices": "Provide a clear target audience and keyword list...",
  "temperature": 0.7,
  "version": "1.0",
  "created": "2026-08-01"
}
```

---

## Prompt Engineering Techniques

PromptVault includes a **complete prompt engineering guide** (in `techniques/`):

| Technique | File | When to Use |
|-----------|------|-------------|
| Chain of Thought (CoT) | `chain-of-thought.md` | Complex reasoning, math, logic |
| Few-shot Prompting | `few-shot.md` | Consistent output format required |
| Tree of Thought | `advanced-techniques.md` | Multi-step problem solving |
| ReAct | `advanced-techniques.md` | Tool use and action planning |
| Self-Consistency | `advanced-techniques.md` | High-accuracy responses |
| System Prompt Design | `claude-system-prompts.md` | Building AI assistants |
| Role Prompting | `prompt-engineering-guide.md` | Persona-based interactions |
| Multi-turn Strategy | `prompt-engineering-guide.md` | Complex conversations |

---

## Model Compatibility Guide

| Model | Best For | Prompt Style Tips |
|-------|----------|-------------------|
| **ChatGPT (GPT-4o)** | General purpose, creative writing | Concise instructions, temperature 0.7 |
| **Claude (Sonnet/Opus)** | Analysis, long-form, reasoning | Detailed system prompts, thinking mode |
| **Gemini** | Multimodal, research, coding | Structured requests, step-by-step |
| **DeepSeek** | Coding, math, Chinese content | Technical specificity, Chinese-friendly |
| **Grok** | Real-time data, casual conversation | Conversational tone, current events |
| **Qwen** | Chinese language, multilingual | Native Chinese prompts work best |

---

## Web Search Tool

`web/index.html` is a standalone search interface. Open it in any browser to:

- Search across all 600+ prompts
- Filter by category, model, difficulty
- View bilingual prompts side-by-side
- Copy prompts with one click
- No server required — works offline

---

## Templates

`templates/` contains ready-to-use system prompt templates:

- `claude-system-prompts.md` — Claude project system prompts
- `gpt-custom-instructions.md` — ChatGPT custom instructions
- `model-specific-tips.md` — Per-model optimization tips

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

1. Fork the repo
2. Add prompts following the JSON schema
3. Ensure both English and Chinese versions
4. Submit a PR with a brief description

---

## Stats

- **600+ prompts** across 12 categories
- **Bilingual** — English + Chinese for every prompt
- **6+ models** supported
- **8 prompt engineering techniques** documented
- **Web search tool** included

---

## Star History

If you find this useful, a ⭐ means a lot!

---

## License

MIT — use freely in any project, personal or commercial.
*（内容由AI生成，仅供参考）*
