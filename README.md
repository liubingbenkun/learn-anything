# Learn Anything

[简体中文](README.zh-CN.md) | English

Learn Anything is a reusable Codex skill for turning any field into a source-grounded, personalized, interactive course.

It is designed for requests such as:

- “Teach me computational neuroscience systematically.”
- “Help me get useful with single-cell RNA-seq in one week.”
- “Use a small set of landmark papers to introduce diffusion models.”
- “I know the basics of economics; help me rebuild the gaps and learn modern causal inference.”

The skill researches the field, identifies the learner's goal and background, builds a dependency-aware curriculum, teaches one coherent idea at a time, and adapts later lessons to the learner's answers.

## Why this skill exists

Many AI-generated courses are expanded outlines: a list of terms, tools, papers, and warnings with little help building intuition. Learn Anything uses a different teaching sequence:

1. Start with what the field is, why it matters, and how it developed.
2. Establish the foundational concepts in the order needed to understand later methods.
3. Introduce terminology, mathematics, tools, and papers only after their motivating problem is clear.
4. Teach through a continuous explanation and sustained examples rather than disconnected definitions.
5. End each lesson with purposeful questions that test explanation, causal reasoning, and transfer.
6. Use the learner's answers to repair misconceptions and adjust the next lesson.

The goal is not merely to produce a syllabus. It is to help a learner form a usable mental model of a field.

## Learning modes

Learn Anything supports five modes that can be combined:

| Mode | Best for |
|---|---|
| Comprehensive | Building durable, field-wide understanding |
| Quick start | Reaching practical competence through the shortest coherent route |
| Project-led | Learning concepts shortly before they are needed in a real project |
| Paper-led | Entering a field through landmark and current papers |
| Refresher | Diagnosing and rebuilding weak or outdated areas |

## How it works

### 1. Research the field

The agent builds a compact evidence map covering the field's central questions, prerequisites, historical transitions, major approaches, representative achievements, applications, open questions, and disagreements. Current or unstable claims are checked against primary or authoritative sources.

### 2. Design the learning route

The curriculum follows conceptual dependencies instead of mirroring a tool catalog. It normally begins with field orientation and foundations, then moves through mechanisms, method families, applications, evaluation, and independent synthesis.

### 3. Teach for understanding

Lessons open with a concrete question, phenomenon, historical episode, or result. Intuition comes before formal terminology. Equations are introduced only when they clarify a problem, and each important term is interpreted in plain language.

### 4. Interact and adapt

Each lesson ends with three or four questions, usually including:

- a teach-back question in the learner's own words;
- a causal or comparative question;
- a transfer or prediction question in a new setting;
- an optional advanced question when appropriate.

The next lesson begins from the learner's actual understanding rather than assuming the previous material was absorbed.

### 5. Organize materials when requested

For an ongoing course, the skill can maintain learning notes, a source index, and a local library of legally accessible papers or official materials. Failed or paywalled downloads are explicitly marked for manual retrieval.

## Installation

Clone the repository into your Codex skills directory:

### macOS and Linux

```bash
git clone https://github.com/liubingbenkun/learn-anything.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/research-and-learn"
```

### Windows PowerShell

```powershell
git clone https://github.com/liubingbenkun/learn-anything.git `
  "$env:USERPROFILE\.codex\skills\research-and-learn"
```

Open a new Codex task after installation so the skill is discovered.

## Usage

Invoke the skill explicitly with `$research-and-learn`:

```text
Use $research-and-learn to teach me computational neuroscience systematically.
I have a machine-learning background but limited neuroscience training.
```

```text
Use $research-and-learn to help me get started with single-cell RNA-seq in one week.
Focus on understanding method choices rather than environment setup.
```

```text
Use $research-and-learn to introduce diffusion models through five key papers.
Fill prerequisite gaps before each paper.
```

```text
Use $research-and-learn to refresh my statistics knowledge for causal inference.
Diagnose what I already understand and skip fluent areas.
```

The skill may also trigger implicitly when a user asks for a systematic learning route, an adaptive course, a field knowledge map, or a paper-led introduction.

## Repository structure

```text
learn-anything/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── curriculum-modes.md
│   ├── research-and-sources.md
│   └── teaching-and-interaction.md
├── README.md
├── README.zh-CN.md
└── LICENSE
```

- `SKILL.md` defines the core workflow and quality gate.
- `curriculum-modes.md` describes course modes and route design.
- `research-and-sources.md` defines research, verification, downloads, and note organization.
- `teaching-and-interaction.md` defines lesson construction, language quality, questions, and adaptive feedback.
- `agents/openai.yaml` contains Codex UI metadata.

## Design principles

- Understanding before coverage.
- Concepts before tools.
- Intuition before formalism.
- Primary and authoritative sources for research claims.
- Complete, fluent explanations rather than fragmented outline prose.
- Questions that reveal mental models rather than test trivia.
- Critical reading after the learner can first explain the method positively.
- Honest uncertainty and multiple viewpoints where the field is unsettled.

## Contributing

Issues and pull requests are welcome. Useful contributions include realistic course examples, improvements to adaptive questioning, clearer source-management procedures, and fixes for failure modes observed during actual teaching.

When proposing a change, explain the learning problem it solves and, where possible, include an example prompt and before/after behavior.

## License

MIT License. See [LICENSE](LICENSE).
