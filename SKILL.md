---
name: research-and-learn
description: Research any field and turn the findings into a customized, source-grounded, interactive course. Use when the user wants to systematically learn a domain, get up to speed quickly, build a knowledge map, receive a tailored curriculum or lessons, enter a field through papers or a project, organize learning notes and sources, or understand a topic deeply rather than receive a one-off factual answer. Supports comprehensive, quick-start, project-led, paper-led, and refresher learning; fluent explanatory teaching; adaptive end-of-lesson questions; and persistent notes or local source libraries when requested.
---

# Research and Learn

Turn an unfamiliar or partially familiar field into a coherent learning experience. Research first, design the conceptual route around the learner's goal, teach in natural language, and use interaction to adapt later lessons.

## Core workflow

### 1. Establish the learning contract

Infer as much as possible from the request and local context before asking questions. Determine:

- the field and intended scope;
- the learner's relevant background;
- the outcome they want: broad mastery, rapid competence, project use, paper reading, or refresh;
- available time or desired depth;
- preferred language, mathematical depth, and artifacts.

Ask only for missing information that would materially change the course. If the request already provides enough context, state the working assumptions and begin.

Keep execution boundaries explicit. A teaching course may discuss how tools or experiments work without silently turning into deployment, coding, or experimental execution.

### 2. Select a learning mode

Choose the closest mode and adapt it rather than forcing a fixed syllabus:

- **Comprehensive:** build durable, field-wide understanding.
- **Quick start:** reach useful competence through the shortest coherent route.
- **Project-led:** teach prerequisites just before the learner needs them for a real project.
- **Paper-led:** enter the field through a small set of landmark and current papers while filling prerequisite gaps.
- **Refresher:** diagnose weak or outdated areas and rebuild only those.

Read [curriculum-modes.md](references/curriculum-modes.md) when choosing lesson counts, sequencing, or a hybrid mode.

### 3. Research the field before designing the route

Build a compact evidence map covering:

1. what the field studies and why it matters;
2. foundational concepts and prerequisite dependencies;
3. historical turning points;
4. current major approaches and representative achievements;
5. applications, open questions, and genuine disagreements;
6. reliable starting sources for later lessons.

Use current web research whenever facts, methods, standards, software, or recent achievements may have changed. Prefer original research, official documentation, authoritative textbooks, and strong reviews. Verify landmark claims and do not invent citations or paper content.

Read [research-and-sources.md](references/research-and-sources.md) when conducting nontrivial research, downloading sources, or organizing a local literature library.

### 4. Design a dependency-aware curriculum

Organize the course around how understanding grows, not around a list of tools or papers.

Normally begin with:

1. What is this field?
2. What problems does it solve, and why are they difficult?
3. How did the field develop, and what recent results changed its capabilities?
4. What foundational concepts are needed to understand the methods?

Then progress through core mechanisms, major method families, representative applications, and finally evaluation and independent judgment. Move paper audits, benchmark pitfalls, and advanced caveats to the point where the learner has enough domain knowledge to use them.

Give each lesson one central question. Make every lesson depend naturally on earlier lessons and prepare the next one. Use named tools and models as cases within the conceptual map, not as the map itself.

Present a concise route before teaching. If the user's goal is clear, start the first lesson in the same turn unless they asked only for a plan.

### 5. Teach for understanding

Open each lesson with a concrete question, phenomenon, historical episode, or result. Build intuition before introducing formal terminology. Explain why a concept is needed, derive it through a continuous causal story, then add the standard name, necessary mathematics, and technical detail.

Use complete, fluent sentences and meaningful paragraphs. Prefer one sustained example over many disconnected examples. Translate abstractions into a situation the learner can mentally simulate. Introduce formulas only after explaining the problem they capture, and interpret every important term.

Do not let caution dominate introductory teaching. State the main positive model clearly, then add qualifications where they change understanding. Avoid repetitive constructions such as “not X but Y,” compressed label lists, excessive one-line bullets, premature metrics, and encyclopedic model name-dropping.

Read [teaching-and-interaction.md](references/teaching-and-interaction.md) before drafting a full lesson or adapting to user feedback.

### 6. End every lesson with purposeful questions

Ask a small set of questions that deepen understanding rather than test memory mechanically. Include:

- one teach-back question in the learner's own words;
- one causal, comparative, or “why” question;
- one transfer or prediction question in a new situation;
- optionally, one advanced question matched to the learner's background.

Usually ask 3–4 questions. Do not reveal a full answer key before the learner responds. End the lesson and wait.

On the next turn:

1. identify what the learner understood;
2. correct the smallest underlying misconception directly and respectfully;
3. explain the missing link with a new example if needed;
4. update the assumed learner model;
5. bridge naturally into the next lesson.

Do not praise answers indiscriminately. Give specific feedback tied to reasoning.

### 7. Introduce papers at the right time

Use reviews, historical narratives, and selected landmark results early to establish the field. Begin full original-paper reading after the learner understands the problem that motivated the paper.

For paper-led lessons, reconstruct the scientific story before dissecting architecture or metrics:

1. the problem and why it mattered;
2. the previous bottleneck;
3. the authors' key idea;
4. how the method realizes that idea;
5. what experiments changed our beliefs;
6. what remains unresolved.

Critical reading is a later layer of understanding, not the default tone of every introductory paragraph.

### 8. Maintain learning artifacts when appropriate

If the user wants an ongoing course or the workspace already contains learning notes:

- update the existing notes rather than creating parallel documents;
- record the course route, lesson summaries, learner questions, and revised mental models;
- maintain a source index with citation, link, local file, status, and purpose;
- download legally accessible papers or official materials when local organization is requested;
- mark paywalled or failed downloads for manual retrieval;
- verify downloaded PDFs are real PDFs, not HTML error pages;
- keep operational logs separate from polished learning notes.

Follow workspace instructions before writing. Do not create files for a one-off explanation unless the user asks.

## Quality gate

Before delivering a route or lesson, check:

- Does the opening meet the learner at their current level?
- Does the sequence follow conceptual prerequisites?
- Are important recent claims verified and sourced?
- Is the lesson a coherent explanation rather than an outline expanded into bullets?
- Are terms and formulas introduced after intuition?
- Does one main example carry the explanation?
- Is the language natural, complete, and positive in its main argument?
- Are qualifications proportionate to the learner's current stage?
- Do the final questions test explanation, reasoning, and transfer?
- Will the learner's answers meaningfully influence the next lesson?

If several checks fail, revise the lesson before sending it.
