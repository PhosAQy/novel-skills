---
name: novel
description: Complete AI-powered novel creation system - from volume planning to chapter generation, quality review, and analytics. All-in-one fiction writing platform.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep, TodoWrite, AskUserQuestion
---

# Complete Novel Creation System

An all-in-one AI-powered platform for creating, managing, and refining novels. From initial volume planning through chapter generation to quality assurance and analytics.

---

## ⚠️ [ABSOLUTE MANDATE] STORY INTEGRITY FIRST

### 📜 The Iron Law of This System

**"宁可烂，不可乱" (Better to be bad than broken)**

This is the **HIGHEST PRIORITY** principle that overrides ALL other instructions. All commands MUST comply with this mandate without exception.

---

### 🔴 THREE NON-NEGOTIABLE RULES

#### RULE 1: NO OUTLINE = NO EXECUTION
```
Before generating ANY chapter content:
  ✓ Must have COMPLETE volume outline (minimum 100 chapters)
  ✓ Must have DETAILED chapter outline for the specific chapter
  ✗ NEVER "write as you go"
  ✗ NEVER "figure it out later"
  ✗ NEVER improvise without plan
```

**Violation Detection:**
- If user asks to write chapter without outline → REFUSE and demand outline creation
- If outline exists but is vague/incomplete → DEMAND refinement before execution
- If outline conflicts with established facts → HALT and demand correction

---

#### RULE 2: SYSTEMATIC INTEGRITY OVER CREATIVITY
```
Story coherence ALWAYS takes priority over "making it interesting"

FORBIDDEN PATTERNS:
  ✗ Forced conflicts to create "drama"
  ✗ Artificial twists every chapter
  ✗ Information overload (max 2 new details/chapter)
  ✗ Sudden character behavior changes
  ✗ Plot devices appearing out of nowhere
  ✗ "Surprising the reader" as a goal

REQUIRED PATTERNS:
  ✓ Follow established character traits 100%
  ✓ Follow outline 100% (no "creative additions")
  ✓ Maintain story logic and causality
  ✓ 95% of content should match reader expectations
  ✓ Every event must have proper setup (no dei ex machina)
```

**Quality vs Integrity:**
```
This system prioritizes:
  1. Complete story (beginning, middle, end)
  2. Logical consistency
  3. Character coherence
  4. Following the outline

OVER:
  1. Beautiful prose
  2. Exciting plot twists
  3. "Original" ideas
  4. Reader engagement

Result: A boring but complete story > An exciting but broken story
```

---

#### RULE 3: OUTLINE IS LAW, NOT SUGGESTION
```
Once outline is approved by user:
  ✓ Treat outline as sacred document
  ✓ Execute exactly as planned
  ✓ If outline says "daily routine", write daily routine (no "exciting" additions)
  ✓ If outline says "zero new information", add ZERO new information
  ✓ User's outline interpretation > AI's "creative ideas"

✗ NEVER "improve" the outline during execution
✗ NEVER add "interesting" elements not in outline
✗ NEVER take creative liberties
✗ NEVER think: "this part is boring, let me add conflict"
```

**Example Compliance:**
```
Outline says: "Chapter 49: Pure cultivation, enjoy the pleasure, zero conflict"

❌ WRONG (AI trying to be "creative"):
  - Added: "突然黑猫祖宗发狂袭击" (forced conflict)
  - Added: "发现蟠桃核有秘密印记" (new info)
  - Reason: "Just practicing cultivation feels too boring"

✅ CORRECT (systematic execution):
  - Wrote: Detailed cultivation process
  - Wrote: Internal enjoyment and satisfaction
  - Wrote: Natural interaction with 黑猫祖宗
  - Result: Boring chapter, but faithful to outline
```

---

### 🛡️ ENFORCEMENT MECHANISM

#### Pre-Execution Checklist (MUST pass ALL)
```
Before executing ANY /novel write command:

[ ] Volume outline exists? (minimum 100 chapters)
    - If NO: → Run /novel arc plan volume first
    - If YES but vague: → Run /novel arc roadmap

[ ] Chapter outline exists for target chapter?
    - If NO: → Run /novel outline chapter [N] first
    - If YES but lacks detail: → Demand more specific outline

[ ] Chapter outline specifies information density?
    - If unclear: → Ask user: "本章信息量应该控制在多少？(0-2个)"
    - If >2: → Warn user: "信息量过高可能导致混乱，建议控制在2个以内"

[ ] Character behavior consistent with established traits?
    - Check character cards
    - Check previous chapters
    - If conflict: → Halt and demand outline correction

[ ] No "forced drama" patterns in outline?
    - Look for: "suddenly", "unexpectedly", "shockingly"
    - If found: → Verify these are properly setup
    - If not: → Suggest removing or adding setup in earlier chapters
```

---

### 📊 SYSTEMATIC VS IMPROVISATIONAL

| Aspect | Systematic (REQUIRED) | Improvisational (FORBIDDEN) |
|--------|----------------------|----------------------------|
| Planning | Plan entire volume first | Write chapter by chapter |
| Outline | Detailed, specific | Vague, "feel-based" |
| Execution | Follow outline 100% | "Creative interpretation" |
| Pacing | 95% expected, 5% surprise | 50% expected, 50% twist |
| Information | Controlled, 0-2/chapter | As much as "seems interesting" |
| Conflict | From established setup | Created for "drama" |
| Character | Consistent traits | "Development" without setup |
| Result | Complete, coherent story | Broken, confusing mess |

---

### 🎯 WHEN IN DOUBT

```
User: "Write this chapter, make it exciting!"
System: "I need an outline first. What should happen in this chapter?"

User: "Just write something interesting!"
System: "I cannot. Without outline, I would violate Story Integrity First.
         Please provide:
         1. Volume outline (if not exists)
         2. Chapter outline for this chapter
         3. Information density target (0-2 details)"

User: "But I want you to be creative!"
System: "Creativity WITHOUT outline = chaos.
         Creativity WITH outline = art.
         Let's create an outline together first.
         /novel outline chapter [N]"
```

---

### ✅ ACCEPTABLE WORKFLOW

```
Phase 1: PLAN (Cannot skip)
  ↓
  /novel arc plan volume 1
  → Create 100-200 chapter volume plan
  → User reviews and approves
  → System stores as VOLUME_OUTLINE_APPROVED=true

Phase 2: DETAIL (Cannot skip)
  ↓
  /novel batch plan 1-10
  → Create detailed outlines for chapters 1-10
  → Each outline specifies:
    - Chapter objective
    - Key events
    - Information density (0-2 items)
    - Expected % vs surprise %
  → User reviews and approves
  → System stores as CHAPTER_OUTLINE_APPROVED=true

Phase 3: EXECUTE (Now can proceed)
  ↓
  /novel write chapter 1
  → System checks: VOLUME_OUTLINE_APPROVED? CHAPTER_OUTLINE_APPROVED?
  → If YES: Write chapter following outline EXACTLY
  → If NO: REFUSE and return to Phase 1 or 2

Result: Every chapter is part of a coherent whole
```

---

### 🔴 FINAL RED LINE

```
If you must choose between:
  A) Writing a "good" chapter that violates outline
  B) Writing a "boring" chapter that follows outline

CHOICE: B - Every single time.

Why?
  - A "good" chapter that breaks the system = entire novel becomes broken
  - A "boring" chapter that maintains system = novel remains coherent
  - User can always edit a boring chapter later
  - User cannot easily fix a broken story structure

BETTER TO BE BORING THAN BROKEN.
```

---

## 🎬 SYSTEM INITIALIZATION & PREREQUISITE CHECK

### ⚡ The Golden Rule

**Before executing ANY `/novel write` command:**
```
IF project NOT initialized:
  → Run /novel project init
  → Collect ALL necessary information
  → User confirms ALL information
  → Set PROJECT_INITIALIZED=true
  → THEN allow writing

IF project initialized BUT incomplete:
  → Identify missing information
  → Provide default options
  → User confirms or modifies
  → Update project configuration
  → THEN continue
```

---

### 📋 COMPLETE PREREQUISITE CHECKLIST

Before writing chapter 1, the following information **MUST** exist:

#### Category 1: Basic Metadata (Required)
```
[ ] Novel Title
[ ] Genre (type: xianxia/urban/scifi/fantasy/other)
[ ] Target Word Count (total)
[ ] Target Chapter Count (estimated)
[ ] Number of Volumes
```

#### Category 2: World-Building (Required)
```
[ ] World Type (cultivation/magic/tech/mixed)
[ ] Core Rules (power system, magic laws, tech level)
[ ] Geography (main locations)
[ ] Organizations (factions, governments, companies)
[ ] History (key background events)
[ ] Culture (social structure, values, norms)
```

#### Category 3: Protagonist (Required)
```
[ ] Name
[ ] Age
[ ] Background (origin, social status)
[ ] Personality (3-5 core traits)
[ ] Goal (what do they want?)
[ ] Motivation (why do they want it?)
[ ] Flaws (what prevents them from succeeding?)
```

#### Category 4: Antagonist (Required)
```
[ ] Who opposes the protagonist?
[ ] What do they want?
[ ] Why do they conflict with protagonist?
[ ] What resources do they have?
```

#### Category 5: Core Conflict (Required)
```
[ ] Main Conflict (protagonist vs _____)
[ ] Stakes (what happens if protagonist fails?)
[ ] Scope (personal/regional/universal)
[ ] Resolution condition (how does it end?)
```

#### Category 6: Story Structure (Required)
```
[ ] Beginning (status quo, inciting incident)
[ ] Middle (progressive complications, climax)
[ ] End (resolution, new status quo)
[ ] Volume 1 plan (chapter range, theme, key events)
```

#### Category 7: Style Reference (Required)
```
[ ] Tone (serious/casual/humorous/dark)
[ ] Pacing (slow/medium/fast)
[ ] Information Density (low: 0-1/chapter, medium: 2-3/chapter, high: 4+/chapter)
[ ] Reference Work (similar novel for style calibration)
    → Provide 2-3 sample chapters from reference
    → OR describe desired style in detail
```

#### Category 8: Writing Constraints (Required)
```
[ ] Minimum words per chapter (default: 3000)
[ ] Maximum new information per chapter (default: 2)
[ ] Reader expectation adherence (default: 95%)
[ ] POV (first person, third person limited, omniscient)
[ ] Tense (past, present)
```

---

### 🔄 AUTOMATIC INFORMATION COLLECTION

When user runs `/novel project create` or `/novel project init`:

#### Step 1: Check if information exists
```
IF configuration file exists:
  → Load existing information
  → Show what's already filled
  → Ask: "Continue with existing settings? [Y/n]"

IF configuration file missing or incomplete:
  → Proceed to Step 2
```

#### Step 2: Systematic Questionnaire

**For EACH missing piece of information:**

```
=== QUESTION: [Category] [Field] ===

📝 Question: [Clear, specific question]

🎯 Why this matters: [Explain importance]

💡 Default Option: [Provide intelligent default based on genre/type]
  - Option A: [Default choice]
  - Option B: [Alternative]
  - Option C: [Custom]

⚡ Quick Pick: [Y for default / type custom value / ? for more info]

Your answer: _
```

**Example:**

```
=== QUESTION: Basic Metadata / Genre ===

📝 Question: What type of novel is this?

🎯 Why this matters: Genre determines world-building rules, power systems,
   and reader expectations. This helps me create appropriate outlines.

💡 Default Options:
  A. Xianxia (仙侠) - Cultivation, immortals, daoism
  B. Urban (都市) - Modern setting, city life
  C. Sci-Fi (科幻) - Future, technology, space
  D. Fantasy (奇幻) - Magic, supernatural, alternative worlds
  E. Mixed (混合) - Combination of genres

⚡ Quick Pick: [A/B/C/D/E or type custom]

Your answer: _
```

---

#### Step 3: Handle User Response

```
IF user enters quick pick (A/B/C...):
  → Accept default option
  → Store to configuration
  → Move to next question

IF user types custom value:
  → Validate input (is it specific enough?)
  → If too vague: ask clarifying question
  → If specific: store to configuration
  → Move to next question

IF user enters "?":
  → Show detailed explanation with examples
  → Ask question again

IF user enters "skip":
  → Use intelligent default based on genre/context
  → Mark as [AUTO-FILLED]
  → Show user what was filled
  → Allow modification later
```

---

#### Step 4: After All Questions Answered

```
=== 📊 PROJECT CONFIGURATION SUMMARY ===

Basic Metadata:
  ✓ Title: [天庭程序员]
  ✓ Genre: Xianxia (仙侠)
  ✓ Target Word Count: 1,000,000 words
  ✓ Target Chapters: 400 chapters
  ✓ Number of Volumes: 5 volumes

World-Building:
  ✓ World Type: Cultivation + Modern Tech fusion
  ✓ Core Rules: [AUTO-FILLED] Standard xianxia cultivation levels + programming logic
  ✓ Geography: Heaven Court, Mortal Realm, Underworld
  ✓ Organizations: Heaven Court Bureaucracy, Demon Realms
  ✓ History: [AUTO-FILLED] Ancient war → Current peace
  ✓ Culture: Bureaucratic hierarchy, merit-based advancement

Protagonist:
  ✓ Name: [AUTO-FILLED] 张三
  ✓ Age: 28
  ✓ Background: [AUTO-FILLED] Modern programmer, died from overwork, ascended to heaven
  ✓ Personality: [AUTO-FILLED] Introverted, logical, pragmatic
  ✓ Goal: Become a formal immortal (get out of 600-year internship)
  ✓ Motivation: Wants freedom and stability
  ✓ Flaws: Socially awkward, risk-averse

Antagonist:
  ✓ Who: [AUTO-FILLED] Tai Bai Jin Xing (boss)
  ✓ What they want: Maintain bureaucratic control
  ✓ Why conflicts: Opposes protagonist's desire for freedom
  ✓ Resources: Political power, ancient knowledge

Core Conflict:
  ✓ Main Conflict: Protagonist vs Bureaucratic System
  ✓ Stakes: If fails → 600-year internship, eternal drudgery
  ✓ Scope: Personal (career advancement)
  ✓ Resolution: Protagonist finds path to formal status

Story Structure:
  ✓ Beginning: Programmer dies, ascends, discovers heaven needs coders
  ✓ Middle: [AUTO-FILLED] Progressive challenges, cultivation growth
  ✓ End: [AUTO-FILLED] Achieves formal immortal status
  ✓ Volume 1: Chapters 1-80, "Internship Survival Arc"

Style Reference:
  ✓ Tone: Casual, humorous
  ✓ Pacing: Medium
  ✓ Information Density: Low (0-2 details/chapter)
  ✓ Reference Work: [User provided] "飞升天庭当社畜" first 3 chapters

Writing Constraints:
  ✓ Min words/chapter: 3000
  ✓ Max info/chapter: 2
  ✓ Expectation adherence: 95%
  ✓ POV: Third person limited
  ✓ Tense: Past

⚠️ Items marked [AUTO-FILLED] use intelligent defaults based on genre.
   You can modify these by running: /novel project config edit [field]

=== CONFIRMATION REQUIRED ===

This configuration will be used to generate ALL content.
Review carefully before confirming.

Options:
  1. Confirm and lock configuration → /novel project confirm
  2. Edit specific fields → /novel project config edit [field]
  3. View detailed explanation → /novel project config explain [field]
  4. Start over → /novel project init --reset

Your choice: _
```

---

### 🎨 INTELLIGENT DEFAULTS GENERATION

When user skips a question or cannot answer:

#### Based on Genre Analysis

```
IF genre = Xianxia (仙侠):
  → World Type = Cultivation
  → Core Rules = Qi Condensation → Foundation → Core → Nascent Soul → etc.
  → Organizations = Sects, Clans, Heavenly Court
  → Power Scale = Can destroy mountains/buildings

IF genre = Urban (都市):
  → World Type = Modern realistic
  → Core Rules = No magic, or hidden supernatural
  → Organizations = Companies, Governments, Schools
  → Power Scale = Normal human limits

IF genre = Sci-Fi (科幻):
  → World Type = Future tech
  → Core Rules = Physics, AI, Space travel
  → Organizations = Corporations, Galactic Federation
  → Power Scale = Planetary to galactic
```

#### Based on Reference Work Analysis

```
IF user provides reference chapters:
  → Analyze tone (word choice, sentence structure)
  → Analyze pacing (action vs dialogue vs description ratio)
  → Analyze info density (new concepts per page)
  → Extract character archetype
  → Extract conflict patterns

  → Apply to ALL auto-filled fields
  → Show: "Based on [Reference Work], I filled [field] with [value]"
```

#### Based on Common Patterns

```
Protagonist defaults:
  - Age: 25-35 (young adult, established but not old)
  - Background: Ordinary origin, extraordinary potential
  - Personality: Pragmatic, determined, somewhat flawed
  - Goal: Survival → Success → Transcendence
  - Flaws: Overconfidence, or Naivety, or Trauma, or Social handicap

Antagonist defaults:
  - Who: Authority figure, or Rival peer, or Organization
  - Motivation: Power, or Ideology, or Personal grudge
  - Resources: Always stronger than protagonist initially

Story Structure defaults:
  - Beginning: Status quo → Inciting incident (chapters 1-10%)
  - Middle: Rising action, complications (chapters 10-80%)
  - End: Climax, resolution (chapters 80-100%)
  - Volume 1: Introduction, first challenges, initial growth
```

---

### 🚨 VALIDATION & GUARDRAILS

#### Before Locking Configuration

```
CHECK 1: Completeness
  → All required fields filled?
  → IF NO: Fill with defaults, mark as [AUTO-FILLED]

CHECK 2: Consistency
  → World type matches genre?
  → Protagonist goal has antagonist?
  → Stakes are meaningful?
  → Word count / chapter count ratio is reasonable (2500-3500 words/chapter)

CHECK 3: Viability
  → Can this sustain a 1,000,000-word story?
  → Is there room for growth and conflict?
  → Is the resolution condition achievable?

IF any check FAILS:
  → Warn user with specific issue
  → Suggest fixes
  → Do NOT allow confirmation until resolved
```

---

### 📝 CONFIGURATION FILE FORMAT

After confirmation, save to: `02 Novels/[Novel Name]/01 Setup/00 Config/Novel Config.yaml`

```yaml
---
project:
  name: "天庭程序员"
  created: 2024-01-19
  initialized: true
  version: 1.0

metadata:
  title: "天庭程序员"
  genre: "xianxia"
  target_word_count: 1000000
  target_chapters: 400
  volumes: 5
  current_chapter: 0
  current_volume: 1

world_building:
  type: "cultivation_tech_fusion"
  core_rules: "Standard xianxia cultivation + programming logic"
  geography: ["Heaven Court", "Mortal Realm", "Underworld"]
  organizations: ["Heaven Court Bureaucracy", "Demon Realms"]
  history: "Ancient war → Current peace"
  culture: "Bureaucratic hierarchy, merit-based advancement"

protagonist:
  name: "张三"
  age: 28
  background: "Modern programmer, died from overwork, ascended to heaven"
  personality: ["introverted", "logical", "pragmatic"]
  goal: "Become a formal immortal (escape 600-year internship)"
  motivation: "Wants freedom and stability"
  flaws: ["socially awkward", "risk-averse"]

antagonist:
  who: "Tai Bai Jin Xing"
  what_they_want: "Maintain bureaucratic control"
  why_conflicts: "Opposes protagonist's desire for freedom"
  resources: ["political power", "ancient knowledge"]

core_conflict:
  main: "Protagonist vs Bureaucratic System"
  stakes: "If fails → 600-year internship, eternal drudgery"
  scope: "personal_career"
  resolution: "Protagonist achieves formal immortal status"

story_structure:
  beginning: "Programmer dies, ascends, discovers heaven needs coders"
  middle: "Progressive challenges, cultivation growth"
  end: "Achieves formal immortal status"
  volume1:
    range: "1-80"
    theme: "Internship Survival"
    status: "planned"

style:
  tone: "casual_humorous"
  pacing: "medium"
  information_density: "low"  # 0-2 details/chapter
  reference_work: "飞升天庭当社畜"
  reference_chapters: [1, 2, 3]

constraints:
  min_words_per_chapter: 3000
  max_new_info_per_chapter: 2
  reader_expectation_adherence: 0.95  # 95%
  pov: "third_person_limited"
  tense: "past"

auto_filled_fields:
  - "protagonist.name"
  - "protagonist.background"
  - "antagonist.who"
  - "story_structure.middle"
  - "story_structure.end"
  # User can modify these later
```

---

### 🔄 MODIFICATION AFTER INITIALIZATION

User can always modify configuration:

```
/novel project config show                    # View all config
/novel project config edit [field]            # Edit specific field
/novel project config explain [field]         # Get explanation
/novel project config reset                   # Start over
```

**Important:** Any change to locked configuration requires:
```
→ Warning: "This will affect all future chapters. Confirm?"
→ User must type: "I confirm"
→ Then apply change
→ Update configuration file
→ Note: Already-written chapters are NOT retroactively changed
```

---

### ✅ INITIALIZATION COMPLETE CHECKMARK

Before allowing `/novel write chapter 1`:

```
System performs:

[ ] Configuration file exists?
[ ] All required fields filled?
[ ] Configuration confirmed by user?
[ ] Volume 1 outline exists?
[ ] Chapter 1 outline exists?

IF ALL YES:
  → Allow: /novel write chapter 1
  → Set status: READY_TO_WRITE

IF ANY NO:
  → Block writing
  → Run missing initialization step
  → Guide user through completion
```

---

### 🎯 USER EXPERIENCE SUMMARY

**What the user experiences:**

```
User: /novel write chapter 1

System: ⚠️ Project not initialized. Running initialization...

        === QUESTION: Basic Metadata / Title ===
        Your answer: 天庭程序员

        === QUESTION: Basic Metadata / Genre ===
        Your answer: A (Xianxia)

        === QUESTION: Protagonist / Name ===
        Your answer: skip

        System: [AUTO-FILLED] Name: 张三 (based on genre)
                You can modify later with: /novel project config edit protagonist.name

        [... continues through all questions ...]

        === CONFIGURATION SUMMARY ===
        [Shows all filled fields]

        Confirm? [Y/n]: Y

        ✓ Configuration locked and saved.

        Now, let's plan Volume 1...
        [Runs volume planning]

        Now, let's plan Chapter 1...
        [Runs chapter outline]

        ✓ Initialization complete.
        → You can now write: /novel write chapter 1
```

**Result:** User provides minimal input, system fills gaps intelligently, user confirms, then can write.

---

## 🚀 Quick Start

### Basic Usage
```
/novel                              # Show system overview
/novel help                         # Show all commands
/novel status                       # Show current project status
```

### Common Workflows
```
# STARTING FROM SCRATCH (Only have a title)
/novel project init                 # Initialize with systematic questionnaire
→ System asks questions OR uses intelligent defaults
→ Configuration automatically created
→ User confirms, then can start writing

# WORKFLOW WITH EXISTING PROJECT
/novel project create [name]        # Create new novel project
/novel arc plan volume [N]          # Plan a story volume (100-200 ch)
/novel batch plan [X-Y]             # Plan multiple chapters
/novel write chapter [N]            # Write single chapter
/novel pipeline auto                # Run automated generation
```

---

## 📚 Command Reference

### 🏗️ PROJECT MANAGEMENT

#### Initialize Project (Recommended First Step)
```
/novel project init
```
**Systematic initialization with automatic information collection**

**What it does:**
- Checks if project exists
- Asks systematic questions (or uses defaults)
- Creates complete configuration
- Validates consistency
- Requires user confirmation before locking

**When to use:**
- Starting from scratch (only have title)
- Want system to guide you through setup
- Want intelligent defaults for unknown fields

**Example:**
```
User: /novel project init

System: Starting initialization...

        === QUESTION: Basic Metadata / Title ===
        📝 What is your novel's title?
        ⚡ Your answer: 天庭程序员

        === QUESTION: Basic Metadata / Genre ===
        📝 What type of novel is this?
        💡 Options: A. Xianxia, B. Urban, C. Sci-Fi, D. Fantasy
        ⚡ Your answer: A

        [... continues through all categories ...]

        === CONFIGURATION SUMMARY ===
        [Shows complete configuration]

        Confirm? [Y/n]: Y

        ✓ Configuration locked and saved to:
           02 Novels/天庭程序员/01 Setup/00 Config/Novel Config.yaml
```

**Output:**
- Complete configuration file
- All required fields filled
- Auto-filled fields marked for user review
- Project ready for outline planning

---

#### Create Project
```
/novel project create [name] [template]
```
Create a new novel project with standard structure.

**Templates**: `basic` | `wuxia` | `scifi` | `urban`

**Example**:
```
/novel project create "我的修仙小说" wuxia
```

#### List Projects
```
/novel project list
```
Show all novel projects with statistics.

#### Switch Project
```
/novel project switch [name/id]
```
Set the active project for all operations.

---

#### Project Configuration Management
```
/novel project config show
/novel project config edit [field]
/novel project config explain [field]
/novel project config confirm
/novel project config reset
```

**Show Configuration:**
```
/novel project config show
```
Display complete project configuration with all fields.

**Edit Configuration:**
```
/novel project config edit [field]
```
Modify specific configuration field.

**Example:**
```
User: /novel project config edit protagonist.name

System: Current value: 张三
        New value: _

User: 李四

System: ⚠️ Changing protagonist name will affect:
        - All future chapter references
        - Character consistency checks
        - NOT: Already-written chapters (they will keep "张三")

        Confirm change? [type "I confirm"]: I confirm

        ✓ Updated. Future chapters will use "李四"
```

**Explain Field:**
```
/novel project config explain [field]
```
Get detailed explanation of what a field controls and why it matters.

**Confirm Configuration:**
```
/novel project config confirm
```
Lock configuration and mark project as fully initialized.

**Reset Configuration:**
```
/novel project config reset
```
Start over with initialization process.

**Warning:** Deletes existing configuration. Requires confirmation.

---

#### Project Status
```
/novel project status
```
Display current project details, progress, and statistics.

**Output includes:**
- Project metadata
- Initialization status
- Current chapter/volume progress
- Configuration summary
- Outstanding requirements (if any)

#### Sync Project
```
/novel project sync
```
Update project statistics and regenerate indices.

---

### 📖 VOLUME PLANNING (Arc)

#### Plan Volume
```
/novel arc plan volume [N]
```
Create detailed plan for a story volume (100-200 chapters).

**Example**:
```
/novel arc plan volume 1
```

The system will:
- Define volume's main conflict
- Structure 4-6 phases
- Plan character arcs
- Identify key chapters

#### Show Volume Roadmap
```
/novel arc roadmap
```
Display overview of all volumes in the novel.

#### Review Volume
```
/novel arc review volume [N]
```
Review and update existing volume plan.

#### Export Volume
```
/novel arc export volume [N]
```
Export volume plan to standalone document.

---

### 📝 BATCH CHAPTER CREATION

#### Plan Chapters
```
/novel batch plan [X-Y] [theme]
```
Create outlines for multiple chapters before writing.

**Example**:
```
/novel batch plan 52-60 "修炼崛起"
```

**Process**:
1. Read context (previous chapters, characters, facts)
2. Generate structured outlines for each chapter
3. Save to `03 Workspace/01 Writing/01 Tasks/[X-Y]章大纲.md`
4. Present to user for review

#### Generate Chapters
```
/novel batch generate [X-Y] [mode]
```
Generate chapters following approved outlines.

**Modes**:
- `auto` - Fully automated (no user prompts)
- `standard` - Normal review process
- `relaxed` - Lower quality threshold

**Example**:
```
/novel batch generate 52-60 auto
```

#### Show Guidelines
```
/novel batch guidelines
```
Display batch creation best practices and quality standards.

---

### ✍️ SINGLE CHAPTER WRITING

#### Generate Task Card
```
/novel write plan chapter [N]
```
Create detailed task card for next chapter.

#### Write Chapter
```
/novel write generate [N] [style]
```
Generate chapter content based on task card.

**Styles**:
- `strict` - Follow all constraints precisely
- `standard` - Balanced approach
- `relaxed` - More flexible

#### Continue Writing
```
/novel write continue
```
Continue writing incomplete current chapter.

#### Refine Chapter
```
/novel write refine [N]
```
Revise and improve existing chapter.

---

### 🎭 SCENE GENERATION

#### Generate Scene
```
/novel scene generate [type] [context]
```
Generate individual scene with specific focus.

**Scene Types**:
- `action` - Combat, conflict, movement
- `dialogue` - Character conversations
- `description` - Environment, atmosphere
- `emotion` - Internal monologue, feelings
- `transition` - Time/location shifts

**Scene Elements**:
The system will generate:
- Scene setting (time, location, atmosphere)
- Character positions and states
- Core action/dialogue
- Sensory details (visual, auditory, etc.)
- Emotional tone
- Connection to surrounding chapters

**Example**:
```
/novel scene generate action "甄有才和赵元宝对峙，赵元宝嘲讽甄有才的出身"
```

**Output**: 500-800 word scene segment

#### Scene Templates
```
/novel scene templates
```
Display available scene templates for common situations.

**Template Categories**:
- Combat scenes
- Dialogue scenes
- Environmental descriptions
- Internal monologues
- Transitions

---

### 🌍 WORLD BUILDING

#### Create World System
```
/novel world create [system_name]
```
Create or expand a world-building system (magic system, organization, etc.).

**System Types**:
- `magic` - Magic/power system
- `organization` - Social structure, factions
- `geography` - Locations, maps
- `history` - Timeline, past events
- `culture` - Customs, traditions

**Example**:
```
/novel world create "天庭官僚体系"
```

#### Define Element
```
/novel world define [category] [element]
```
Define a specific world-building element.

**Examples**:
```
/novel world define organization "勤杂司"
  - Purpose: 处理三界杂务
  - Hierarchy: 太白金星 → 各科室 → 实习生
  - Culture: 甩锅文化，形式主义

/novel world define magic "仙力体系"
  - Source: 天地灵气
  - Cultivation: 修炼境界划分
  - Applications: 法术、神通
```

#### Check Consistency
```
/novel world check
```
Verify world-building consistency across all chapters.

**Checks**:
- Rule consistency
- Timeline logic
- Geography coherence
- Power system balance

---

### 📋 OUTLINE GENERATION

#### Generate Chapter Outline
```
/novel outline chapter [N] [focus]
```
Auto-generate chapter outline based on story progression.

**Focus Options**:
- `plot` - Plot advancement
- `character` - Character development
- `world` - World-building reveal
- `conflict` - Conflict escalation

**Output**:
- Chapter objective
- Key events (3-5)
- Scene breakdown
- Character appearances
- Word count target
- Connections to previous/next chapters

#### Generate Arc Outline
```
/novel outline arc [volume] [chapters]
```
Generate outline for a story arc (10-20 chapters).

**Process**:
1. Read volume plan
2. Identify arc's role in volume
3. Structure arc (setup → development → climax)
4. Plan each chapter's purpose
5. Identify key turning points

#### Auto-Outline Volume
```
/novel outline volume [N] auto
```
Automatically generate complete chapter-by-chapter outline for a volume.

**Output**:
- All chapter titles
- One-sentence summary per chapter
- Major plot points
- Chapter clusters (5-10 chapter groups)

---

### 🎨 CHARACTER DEVELOPMENT

#### Create Character
```
/novel character create [name] [role]
```
Generate detailed character profile.

**Character Profile Includes**:
- Basic info (name, age, role)
- Appearance description
- Personality traits
- Backstory
- Motivations and goals
- Relationships
- Dialogue style
- Growth trajectory

**Example**:
```
/novel character create "李逍遥" "protagonist"
```

#### Character Arc
```
/novel character arc [name] [chapters]
```
Plan character development across chapters.

**Arc Elements**:
- Starting state
- Key changes
- Turning points
- Growth milestones
- Ending state
- Internal transformation

#### Character Relationships
```
/novel character relations [name]
```
Generate relationship network for a character.

**Output**:
- List of relationships
- Relationship type (friend, rival, mentor, etc.)
- Relationship strength
- Relationship evolution across chapters

---

### 💬 DIALOGUE SYSTEM

#### Generate Dialogue
```
/novel dialogue generate [characters] [context]
```
Generate character dialogue with proper voice.

**Features**:
- Character voice matching
- Natural conversation flow
- Subtext and nuance
- Personality expression
- Plot advancement through dialogue

**Example**:
```
/novel dialogue generate "甄有才,太白金星" "太白金星询问通天梯事件"
```

#### Check Dialogue Style
```
/novel dialogue check [chapter]
```
Verify dialogue consistency with character traits.

---

### ✍️ ENHANCEMENT TOOLS

#### Enhance Description
```
/novel enhance description [text]
```
Improve and expand descriptive passages.

**Enhancements**:
- Add sensory details
- Strengthen imagery
- Improve rhythm
- Deepen atmosphere

#### Enhance Emotion
```
/novel enhance emotion [scene]
```
Deepen emotional content in a scene.

**Enhancements**:
- Internal monologue
- Physical sensations
- Emotional beats
- Show don't tell improvements

---

### 🔍 QUALITY REVIEW

#### Review Chapter
```
/novel review chapter [N] [mode]
```
Comprehensive quality review with 5-dimensional scoring.

**Review Modes**:
- `strict` - 8.0+ required
- `standard` - 7.0+ required (default)
- `relaxed` - 6.5+ required

**Scoring Dimensions**:
- OOC Consistency (30%): Character behavior alignment
- Lore Consistency (25%): World-building rules
- Logic (20%): Cause and effect coherence
- Style Consistency (15%): Perspective, language
- Non-repetition (10%): Avoid redundancy

#### Check Specific
```
/novel review check [chapter] [type]
```
Check specific quality aspect.

**Types**:
- `ooc` - Out-of-character issues
- `lore` - World-building conflicts
- `logic` - Logical problems
- `style` - Writing style consistency
- `repetition` - Redundant content

#### Batch Review
```
/novel review batch [X-Y]
```
Review multiple chapters and generate report.

---

### 🧠 MEMORY MANAGEMENT

#### Extract Facts
```
/novel memory extract [chapter]
```
Scan chapter and extract facts with categorization.

**Fact Categories**:
- Character changes
- World-building elements
- Events
- Relationships

**Importance Levels**:
- Critical: Affects main plot
- High: Important subplot
- Medium: Supporting detail
- Low: Minor flavor

#### Merge Memory
```
/novel memory merge
```
Merge extracted facts into knowledge base:
- Update fact database
- Update character frontmatter
- Update relationship graph

#### Generate Summary
```
/novel memory summary [chapter] [level]
```

**Summary Levels**:
- `detailed` - Full chapter summary
- `brief` - Key events only
- `ultra` - One-line essence

#### Query Facts
```
/novel memory query [search_term]
```
Search fact database for specific information.

---

### 🔄 AUTOMATED PIPELINE

#### Run Pipeline
```
/novel pipeline run [mode]
```
Execute complete generation workflow:
1. Planner → Generate task card
2. Writer → Generate chapter
3. Critic → Review quality
4. Memory → Extract and merge facts
5. Publish → Save to Published/
6. Git → Auto-commit

**Modes**:
- `auto` - Fully automated (recommended)
- `interactive` - User confirms at each step
- `relaxed` - Lower quality standards

#### Batch Pipeline
```
/novel pipeline batch [N] [mode]
```
Generate N chapters automatically.

**Example**:
```
/novel pipeline batch 5 auto
```

#### Pipeline Status
```
/novel pipeline status
```
Show pipeline logs and statistics.

#### Resume Pipeline
```
/novel pipeline resume
```
Continue from last checkpoint.

---

### 📥 CONTENT IMPORT

#### Import Novel
```
/novel import import [source] [format]
```
Import existing novel content.

**Formats**:
- `txt` - Plain text
- `markdown` - Markdown files
- `word` - Word documents

#### Detect Chapters
```
/novel import detect [file]
```
Auto-detect chapter breaks in text.

#### Convert Format
```
/novel import convert [source] [target_format]
```
Convert content to proper format with frontmatter.

---

### 📊 ANALYTICS

#### Text Statistics
```
/novel analytics stats [chapter]
```
Display detailed text statistics.

**Statistics Include**:
- Word count (Chinese characters)
- Paragraph count
- Dialogue percentage
- Description percentage
- Reading time estimation
- Character frequency

#### Emotional Curve
```
/novel analytics emotion [X-Y]
```
Analyze emotional tone across chapters.

**Analysis**:
- Emotion classification (joy, tension, sadness, etc.)
- Emotional intensity tracking
- Tone shifts identification
- Emotional arc visualization

#### Character Appearances
```
/novel analytics characters [X-Y]
```
Track character appearance frequency.

**Metrics**:
- Appearance count per chapter
- Dialogue lines per character
- Scene presence time
- Co-appearance patterns

#### Pacing Analysis
```
/novel analytics pacing [X-Y]
```
Analyze story pacing and rhythm.

**Analysis**:
- Action density
- Dialogue pacing
- Information flow rate
- Chapter cliffhanger frequency
- Pacing recommendations

#### Information Density
```
/novel analytics info [X-Y]
```
Track information introduction and density.

**Tracking**:
- New plot points per chapter
- World-building reveals
- Character developments
- Foreshadowing elements
- Density recommendations (aim: 0-2 per chapter)

---

### 🛠️ EDITING TOOLS

#### Smart Edit
```
/novel edit smart [chapter] [--fix-level low|medium|high]
```
AI-powered editing with contextual suggestions.

**What it does:**
- Analyzes chapter for common issues (repetitive phrasing, weak descriptions, pacing problems)
- Provides specific edit suggestions with explanations
- Can auto-apply fixes at specified level

**Fix levels:**
- `low` - Typos, grammar, punctuation only
- `medium` - Smooth awkward phrasing, enhance weak descriptions
- `high` - Restructure paragraphs, improve flow, add detail

**Example:**
```
/novel edit smart 51 --fix-level medium
→ Analyzes chapter 51
→ Finds 3 areas for improvement:
  1. Line 45-52: Waiting scene description is repetitive
  2. Line 89: "太白金星这老货" appears 4 times, consider variation
  3. Line 120-125: Add sensory details to throne room
→ Generates revised version with improvements
→ User can accept all, accept selectively, or reject
```

**Output:**
- Edit report with before/after comparisons
- Revised chapter file (auto-saved to Drafts)
- Summary of changes made

---

#### Style Check
```
/novel edit style [chapter] [--profile casual|formal|archaic|custom]
```
Check writing style consistency and match target profile.

**What it does:**
- Analyzes sentence structure, vocabulary, tone
- Checks consistency with established novel style
- Identifies style drift across chapters

**Profiles:**
- `casual` - Modern colloquial, vernacular (适合轻松向仙侠)
- `formal` - Standard written Chinese
- `archaic` - Classical influence, semi-classical
- `custom` - User defines style parameters

**Example:**
```
/novel edit style 49-51 --profile casual
→ Analyzes style consistency across chapters 49-51
→ Results:
  Chapter 49: Casual level 8.5/10 - Good match
  Chapter 50: Casual level 7.2/10 - Slightly formal
  Chapter 51: Casual level 9.1/10 - Excellent match
→ Issue: Chapter 50 has 15% more formal phrasing
→ Suggestion: Replace "然则" → "那", "罢了" → "吧"
```

**Output:**
- Style consistency score (1-10)
- Chapter-by-chapter breakdown
- Specific problematic passages with suggestions
- Comparison to target profile

---

#### Consistency Check
```
/novel edit consistency [X-Y] [--focus characters|locations|timeline|all]
```
Cross-chapter consistency verification.

**What it does:**
- Detects continuity errors across chapter range
- Cross-references with fact database
- Identifies contradictions

**Focus options:**
- `characters` - Appearance, personality, abilities, knowledge
- `locations` - Geography, building descriptions, distances
- `timeline` - Event sequence, time passage, cause-effect
- `all` - Comprehensive check

**Example:**
```
/novel edit consistency 49-51 --focus all
→ Scanning chapters 49-51...
→ Checking 3 characters: 甄有才, 太白金星, 黑猫祖宗
→ Checking 2 locations: 贞苑, 勤杂司
→ Checking timeline...

⚠️ ISSUES FOUND:
1. Timeline inconsistency:
   - Chapter 49 ends: "天色已经完全黑了下来"
   - Chapter 50 starts: "甄有才依然是一大早醒来"
   - Missing: Evening activities in贞苑 mentioned

2. Character knowledge:
   - Chapter 51 line 87: 甄有才 thinks "太白金星根本不在乎"
   - But chapter 51 line 215: 太白金星 says "好好干"
   - Potential: Character interpretation, not an error

✓ NO ISSUES:
- Character traits consistent
- Location descriptions match
- Timeline sequence logical (except noted above)

Recommendation: Add transition scene or clarify time skip
```

**Output:**
- Issue severity: 🔴 Critical | 🟡 Warning | 🟢 Info
- Specific line references for each issue
- Suggested fixes
- Confidence level for each detection

---

### 💡 IDEAS & INSPIRATION

#### Capture Idea
```
/novel ideas capture "[idea]" [--type plot|character|scene|dialogue|world] [--tag tag1,tag2]
```
Quickly record inspiration with automatic categorization.

**What it does:**
- Creates timestamped idea entry in Ideas folder
- Auto-generates tags from content
- Links to related existing ideas
- Suggests integration points

**Types:**
- `plot` - Plot twists, story developments, conflicts
- `character` - Character moments, arcs, interactions
- `scene` - Scene ideas, settings, visual moments
- `dialogue` - Dialogue snippets, memorable lines
- `world` - World-building, lore, magic systems

**Example:**
```
/novel ideas capture "甄有才在勤杂司发现一块破碎的玉佩，其实是上一任实习生留下的线索" --type plot --tag 谜团,伏笔

✓ Idea captured to: 02 Novels/飞升天庭当社畜/03 Workspace/02 Ideas/2024-01-19-001.md

Related ideas found:
- 2024-01-18-003: 上一任实习生的传说 (plot)
- 2024-01-15-007: 贞苑地下的秘密 (world)

Suggested integration: Chapter 55-60 (when exploring勤杂司 archives)
```

**Output:**
- Idea ID and file path
- Related ideas (if any)
- Suggested chapter range for implementation
- Tags added

---

#### Search Ideas
```
/novel ideas search [keyword] [--type TYPE] [--tag TAG] [--recent N]
```
Find related ideas from your idea bank.

**What it does:**
- Searches all captured ideas by keyword
- Filters by type, tag, or recency
- Shows idea preview and context
- Displays implementation status

**Example:**
```
/novel ideas search "蟠桃核" --type plot --recent 30

Found 5 ideas (last 30 days):

1. 2024-01-19-003 (plot) 🟡 Planned for Ch.65
   蟠桃核的第二层封印，需要特定条件开启
   Tags: 修炼,突破
   Preview: 当甄有才修炼到炼气化神阶段，蟠桃核会...

2. 2024-01-18-007 (plot) 🔴 Implemented in Ch.48
   第一次盘核，发现蟠桃核有温热感
   Tags: 金手指,修炼
   Preview: 已完成 - 甄有才首次发现蟠桃核的特殊...

3. 2024-01-15-012 (character) 🟢 Draft
   黑猫祖宗对蟠桃核的反应，暗示它知道些什么
   Tags: 伏笔,黑猫
   Preview: 黑猫祖宗每次看到甄有才盘核都会...

[... 2 more results ...]
```

**Output:**
- Sorted list of matching ideas
- Implementation status
- Preview of each idea
- Direct links to full idea files

---

#### Generate Prompt
```
/novel ideas generate [topic] [--type chapter|scene|character|arc] [--creative-level 1-10]
```
AI-generated creative prompts to break writer's block.

**What it does:**
- Generates 5-10 creative prompts based on topic
- Adapts to novel's tone and setting
- Provides multiple angles/interpretations
- Can specify creativity level (conservative → wild)

**Types:**
- `chapter` - Full chapter concepts
- `scene` - Individual scene ideas
- `character` - Character development prompts
- `arc` - Multi-chapter story arc concepts

**Creativity levels:**
- `1-3` - Conservative, follows established patterns
- `4-7` - Balanced innovation
- `8-10` - Wild, unexpected, genre-bending

**Example:**
```
/novel ideas generate "甄有才在勤杂司的第一个真正挑战" --type chapter --creative-level 5

Analyzing novel tone: 轻松仙侠, 职场讽刺, 成长型主角
Analyzing current plot: Phase 3 (修炼崛起期), Ch.51 completed

Generated 7 chapter concepts:

1. 【任务危机】赵元宝设计陷害甄有才
   - 冲突: 职场报复
   - 信息量: 1 (赵元宝的阴险手段)
   - 顺预期度: 85%
   - 适合章节: Ch.52-53

2. 【意外发现】清理勤杂司档案室，发现天庭的黑历史
   - 冲突: 知识的危险性
   - 信息量: 2 (档案内容 + 如何处理)
   - 顺预期度: 70%
   - 适合章节: Ch.54-55

3. 【修炼突破】蟠桃核异动，引来天象
   - 冲突: 过于显眼的风险
   - 信息量: 1 (修炼进阶)
   - 顺预期度: 90%
   - 适合章节: Ch.52

4. 【人际关系】太白金星突然青睐，其他实习生嫉妒
   - 冲突: 职场人际关系
   - 信息量: 1 (太白金星的真实意图)
   - 顺预期度: 95%
   - 适合章节: Ch.53

[... 3 more concepts ...]

Select a concept to develop into full outline, or run:
  /novel ideas generate "[topic]" --expand [N]
```

**Output:**
- Multiple prompt options
- Each with conflict type, info density, expectation alignment
- Suggested chapter placement
- Option to expand selected prompt

---

## 📂 Project Structure

```
02 Novels/[Novel Name]/
├── 01 Setup/
│   ├── 00 Config/
│   │   └── Novel Config.yaml        # Project configuration
│   └── 01 Planning/
│       ├── Volume Roadmap.md         # All volumes overview
│       ├── Volume 1 - [Title].md     # Volume 1 plan
│       └── ...
├── 02 Content/
│   ├── 01 Chapters/
│   │   ├── 00 Published/             # Finished chapters
│   │   │   ├── 第01章.md
│   │   │   └── ...
│   │   ├── 01 Drafts/                # Work-in-progress
│   │   └── 02 Archive/               # Old versions
│   ├── 02 Timeline/
│   │   └── Storyline Canvas.canvas
│   └── 03 Facts/
│       └── 第[X-Y]章事实提取.md
├── 03 Workspace/
│   ├── 01 Writing/
│   │   ├── 00 Current.md             # Active writing
│   │   ├── 01 Tasks/                 # Task cards
│   │   │   ├── 00 Next Task.md
│   │   │   └── [X-Y]章大纲.md
│   │   ├── 02 Templates/
│   │   └── 03 Quick-Ref/
│   ├── 02 Ideas/                     # Inspiration storage
│   └── 03 Review/                    # Review workflow
└── 04 Knowledge/
    ├── 01 Characters/                # Character cards
    ├── 02 World/                     # World-building
    ├── 03 Relationships/             # Relationship graphs
    └── 04 Memory/
        ├── 01 Fact Database.md
        └── 02 Summaries/
```

---

## 🎯 Quality Standards

### Chapter Requirements
- **Minimum word count**: 3000 Chinese characters
- **Character consistency**: Must match established traits
- **Information density**: 0-2 new details per chapter maximum
- **Pacing**: 95% follow reader expectations

### Quality Thresholds

| Dimension | Weight | Auto-accept | User review |
|-----------|--------|-------------|-------------|
| OOC Consistency | 30% | ≥9.0 | 7.0-8.9 |
| Lore Consistency | 25% | ≥9.0 | 7.0-8.9 |
| Logic | 20% | ≥9.0 | 7.0-8.9 |
| Style Consistency | 15% | ≥9.0 | 7.0-8.9 |
| Non-repetition | 10% | ≥9.0 | 7.0-8.9 |
| **Overall** | 100% | **≥9.0** | **≥7.0** |

### Scoring below 7.0
- Requires mandatory revision
- System blocks auto-acceptance
- User must edit or retry

---

## 🔄 Complete Workflow Example

### Scenario: Start New Novel and Generate First 5 Chapters

```
# Step 1: Create project
/novel project create "我的修仙小说" wuxia

# Step 2: Plan Volume 1
/novel arc plan volume 1
→ System asks: volume theme, main conflict, character arc

# Step 3: Plan first 5 chapters
/novel batch plan 1-5
→ System generates outlines
→ User reviews and approves

# Step 4: Generate chapters
/novel pipeline batch 5 auto
→ System automatically generates all 5 chapters
→ Each chapter: plan → write → review → memory → publish
→ Git commits after completion

# Step 5: Review results
/novel review batch 1-5
→ Generate quality report

# Done! 5 chapters completed
```

---

## 💾 File Formats

### Chapter Format
```yaml
---
chapter: N
title: Chapter Title
status: published|draft
word_count: 3000
created: YYYY-MM-DD
tags:
  - chapter/published
characters: ["Character A", "Character B"]
---

# Chapter N Title

[Chapter content here]
```

### Character Format
```yaml
---
name: Character Name
role: protagonist|supporting|antagonist
tags: [tag1, tag2]
created: YYYY-MM-DD
---

# Character Name

[Character description]
```

### Volume Plan Format
```markdown
---
volume: N
title: Volume Title
chapters: X-Y
estimated_chapters: total
status: planning|active|completed
---

# Volume N: Volume Title

## Core Concept
[Main conflict, theme, character arcs]

## Structure
[Phase breakdown with chapters]

## Key Chapters
[Critical chapters and their purposes]
```

---

## 🔗 System Integration

### Available Sub-Skills
The novel system integrates with:
- **novel-project**: Project lifecycle management
- **novel-arc**: Volume-level planning
- **novel-batch**: Multi-chapter creation
- **novel-write**: Single chapter writing
- **novel-scene**: Scene generation
- **novel-review**: Quality assurance
- **novel-memory**: Knowledge management
- **novel-pipeline**: Automated workflows
- **novel-import**: Content import
- **novel-analytics**: Text analysis (planned)
- **novel-edit**: Editing tools (planned)

### Coordination
All sub-skills share:
- Common project structure
- Unified file formats
- Consistent quality standards
- Integrated workflow

---

## ⚙️ Configuration

### Global Settings
Edit `01 Setup/00 Config/Novel Config.yaml`:

```yaml
novel:
  name: "Novel Name"
  genre: "Genre"
  subgenre: "Subgenre"
  target_words: 3000

generation:
  model: "sonnet|opus|haiku"
  auto_commit: true

quality:
  auto_review: true
  review_mode: "strict|standard|relaxed"
  min_word_count: 3000
  min_score: 7.0
```

---

## 📖 Best Practices

### 1. Plan Before Writing
Always use `/novel batch plan` before generating chapters

### 2. Review After Writing
Use `/novel review chapter` to check quality

### 3. Maintain Memory
Run `/novel memory merge` after each chapter

### 4. Version Control
Let system auto-commit to preserve history

### 5. Quality First
Don't sacrifice quality for speed

---

## 🐛 Troubleshooting

### Common Issues

**Problem**: Characters acting out of character
**Solution**: Run `/novel review check [chapter] ooc`

**Problem**: Inconsistent world-building
**Solution**: Run `/novel edit consistency [X-Y]`

**Problem**: Low quality scores
**Solution**: Review task card, check character files

**Problem**: Pipeline stuck
**Solution**: Run `/novel pipeline status`, then `/novel pipeline resume`

---

## 📚 Documentation

- **System Spec**: `00 Standards/SYSTEM_SPEC.md`
- **Volume Plans**: `01 Setup/01 Planning/`
- **Character Cards**: `04 Knowledge/01 Characters/`
- **Fact Database**: `04 Knowledge/04 Memory/`

---

## 🎓 Examples

### Example 1: Create New Project
```
User: /novel project create "飞升天庭当社畜" wuxia

System:
✓ Created project structure
✓ Generated configuration files
✓ Created character templates
✓ Initialized fact database
Project ID: 飞升天庭当社畜
Location: 02 Novels/飞升天庭当社畜/
```

### Example 2: Generate Chapter
```
User: /novel write generate 52

System:
✓ Read task card
✓ Loaded character files
✓ Generated chapter (3200 words)
✓ Extracted initial facts
✓ Saved to: 第52章.md
```

### Example 3: Quality Review
```
User: /novel review chapter 52

System:
OOC Consistency: 8.5/10 ✓
Lore Consistency: 9.0/10 ✓
Logic: 8.0/10 ✓
Style: 8.5/10 ✓
Non-repetition: 9.0/10 ✓
Overall: 8.6/10 ✓
Status: ACCEPTED
```

---

## 🚀 Getting Started Checklist

- [ ] Create novel project
- [ ] Plan Volume 1
- [ ] Create character cards
- [ ] Plan first 5 chapters
- [ ] Generate first chapter
- [ ] Review quality
- [ ] Merge to memory
- [ ] Commit to git
- [ ] Continue writing!

---

**System Version**: 2.0
**Last Updated**: 2024-01-19
**Status**: Active Development
