# Novel Skills - Claude Code Plugin

Complete AI-powered novel creation system for Claude Code. From volume planning to chapter generation, quality review, and analytics - an all-in-one fiction writing platform.

## Features

- **Project Management**: Initialize, configure, and manage novel projects
- **Volume Planning**: Plan story arcs with 100-200 chapter structures
- **Chapter Generation**: AI-assisted writing with quality control
- **Quality Review**: 5-dimensional scoring system (OOC, Lore, Logic, Style, Repetition)
- **Memory Management**: Automatic fact extraction and knowledge base updates
- **Character Development**: Track characters, relationships, and arcs
- **World Building**: Create and maintain consistent world systems
- **Analytics**: Text statistics, emotional curves, pacing analysis
- **Automated Pipeline**: End-to-end generation workflow

## Installation

### Via Plugin Market (Recommended)

```
/plugin marketplace add PhosAQy/novel-skills
/plugin install novel@novel-skills
```

## Quick Start

Forget everything and just say what you want!!!

## Project Structure

### Novel Project Structure

```
02 Novels/[Novel Name]/
├── 01 Setup/
│   ├── 00 Config/
│   │   └── Novel Config.yaml
│   └── 01 Planning/
│       ├── Volume Roadmap.md
│       └── Volume 1 - [Title].md
├── 02 Content/
│   ├── 01 Chapters/
│   │   ├── 00 Published/
│   │   ├── 01 Drafts/
│   │   └── 02 Archive/
│   ├── 02 Timeline/
│   └── 03 Facts/
├── 03 Workspace/
│   ├── 01 Writing/
│   ├── 02 Ideas/
│   └── 03 Review/
└── 04 Knowledge/
    ├── 01 Characters/
    ├── 02 World/
    ├── 03 Relationships/
    └── 04 Memory/
```

## Core Principles

### Story Integrity First

This plugin follows the principle: **"Better to be bad than broken"** (宁可烂，不可乱)

- **No outline = No execution**: Always plan before writing
- **Systematic integrity over creativity**: Follow outlines 100%
- **Outline is law**: Treat approved outlines as sacred documents
- **95% expectation adherence**: Match reader expectations, avoid forced drama

### Quality Standards

| Dimension | Weight | Auto-accept | User review |
|-----------|--------|-------------|-------------|
| OOC Consistency | 30% | ≥9.0 | 7.0-8.9 |
| Lore Consistency | 25% | ≥9.0 | 7.0-8.9 |
| Logic | 20% | ≥9.0 | 7.0-8.9 |
| Style Consistency | 15% | ≥9.0 | 7.0-8.9 |
| Non-repetition | 10% | ≥9.0 | 7.0-8.9 |
| **Overall** | 100% | **≥9.0** | **≥7.0** |

## Requirements

- Claude Code version 1.0.33 or higher
- Git (for version control)

## License

MIT License - feel free to use this plugin for personal or commercial projects.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## Support

For issues, questions, or suggestions, please:
1. Check the troubleshooting section in the SKILL.md
2. Search existing issues
3. Create a new issue with details

## Version History

- **1.0.0** (2026-01-19): Initial release
  - Complete novel creation system
  - Quality review with 5-dimensional scoring
  - Automated pipeline
  - Memory management
  - Analytics tools

## Acknowledgments

Built with Claude Code Plugin System.
Inspired by the need for systematic, coherent novel creation with AI assistance.
