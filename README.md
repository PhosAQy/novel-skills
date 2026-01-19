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

```bash
claude plugin install novel-skills
```

### Manual Installation

```bash
# Clone this repository
git clone https://github.com/your-username/novel-skills.git

# Install the plugin
claude plugin install ./novel-skills

# Restart Claude Code
```

### Local Development

```bash
# Test the plugin without installing
claude --plugin-dir ./novel-skills
```

## Quick Start

### 1. Initialize Your Novel

```bash
/novel project init
```

This will guide you through a systematic questionnaire to collect:
- Basic metadata (title, genre, word count)
- World-building (rules, geography, organizations)
- Protagonist and antagonist profiles
- Core conflict and story structure
- Style reference and writing constraints

### 2. Plan Volume 1

```bash
/novel arc plan volume 1
```

Create a detailed 100-200 chapter plan for your first volume.

### 3. Outline Chapters

```bash
/novel batch plan 1-10
```

Generate detailed outlines for chapters 1-10 before writing.

### 4. Write Your First Chapter

```bash
/novel write chapter 1
```

Follow the outline exactly to maintain story integrity.

### 5. Review Quality

```bash
/novel review chapter 1
```

Get comprehensive quality feedback with 5-dimensional scoring.

## Project Structure

```
novel-skills/
├── .claude-plugin/
│   └── plugin.json          # Plugin manifest
├── skills/
│   └── novel/
│       └── SKILL.md         # Main novel creation skill
├── README.md                # This file
└── marketplace.json         # Plugin market metadata
```

### Novel Project Structure (Created by Plugin)

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

## Main Commands

### Project Management

```bash
/novel project init              # Initialize with guided setup
/novel project create [name]     # Create new project
/novel project list              # List all projects
/novel project switch [name]     # Switch active project
/novel project status            # Show project details
/novel project config show       # View configuration
/novel project config edit       # Edit configuration
```

### Planning

```bash
/novel arc plan volume [N]       # Plan volume (100-200 chapters)
/novel arc roadmap               # Show volume roadmap
/novel batch plan [X-Y]          # Plan multiple chapters
/novel outline chapter [N]       # Generate chapter outline
```

### Writing

```bash
/novel write chapter [N]         # Write single chapter
/novel write plan chapter [N]    # Generate task card
/novel scene generate [type]     # Generate scene
/novel dialogue generate         # Generate dialogue
```

### Quality Review

```bash
/novel review chapter [N]        # Comprehensive review
/novel review check [N] [type]   # Check specific aspect
/novel review batch [X-Y]        # Review multiple chapters
```

### Memory & Analytics

```bash
/novel memory extract [N]        # Extract facts
/novel memory merge              # Merge to knowledge base
/novel analytics stats [N]       # Text statistics
/novel analytics emotion [X-Y]   # Emotional curve
```

### Automation

```bash
/novel pipeline run [mode]       # Run automated pipeline
/novel pipeline batch [N]        # Generate N chapters
```

## Workflows

### Starting from Scratch

```bash
# 1. Initialize project
/novel project init

# 2. Plan volume
/novel arc plan volume 1

# 3. Plan chapters
/novel batch plan 1-10

# 4. Write chapters
/novel write chapter 1

# 5. Review quality
/novel review chapter 1

# 6. Merge memory
/novel memory merge 1
```

### Automated Generation

```bash
# Generate 5 chapters automatically
/novel pipeline batch 5 auto

# Review batch
/novel review batch 1-5
```

## Configuration

Edit your novel's configuration file:

```yaml
project:
  name: "Novel Name"
  genre: "xianxia"
  target_word_count: 1000000
  target_chapters: 400

constraints:
  min_words_per_chapter: 3000
  max_new_info_per_chapter: 2
  reader_expectation_adherence: 0.95

style:
  tone: "casual_humorous"
  pacing: "medium"
  information_density: "low"
```

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

- **1.0.0** (2024-01-19): Initial release
  - Complete novel creation system
  - Quality review with 5-dimensional scoring
  - Automated pipeline
  - Memory management
  - Analytics tools

## Acknowledgments

Built with Claude Code Plugin System.
Inspired by the need for systematic, coherent novel creation with AI assistance.
