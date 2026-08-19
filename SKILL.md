---
name: learn-anything
description: Research any field and turn the findings into a customized, source-grounded, interactive course. Use when the user wants to systematically learn a domain, get up to speed quickly, build a knowledge map, receive a tailored curriculum or lessons, enter a field through papers or a project, organize learning notes and sources, or understand a topic deeply rather than receive a one-off factual answer. Supports comprehensive, quick-start, project-led, paper-led, and refresher learning; fluent explanatory teaching; adaptive end-of-lesson questions; and persistent notes or local source libraries when requested.
---

# Learn Anything

Turn an unfamiliar or partially familiar field into a coherent learning experience. Research first, design the conceptual route around the learner's goal, teach in natural language, and use interaction to adapt later lessons.

## Core workflow

### 1. Establish a provisional learner profile

Infer as much as possible from the request and local context before asking questions. Determine:

- the field and intended scope;
- the learner's relevant background;
- the outcome they want: broad mastery, rapid competence, project use, paper reading, or refresh;
- available time or desired depth;
- preferred language, mathematical depth, and artifacts.

Ask only for information needed to begin reconnaissance. Treat this profile as provisional: learners often cannot choose a useful course shape until they have seen a clear overview of the field.

Keep execution boundaries explicit. A teaching course may discuss how tools or experiments work without silently turning into deployment, coding, or experimental execution.

### 2. Research and orient before fixing the curriculum

Build a compact evidence map, then give the learner a short, accessible orientation covering the field's purpose, main problem and method families, minimum prerequisites, historical turning points, representative current achievements, and the kinds of theoretical, paper-based, and hands-on study the field supports. Keep this informative enough for a real choice but shorter than a full lesson.

### 3. Offer route choices and ask for direction

Do not silently turn the research map into a fixed syllabus. Propose 2–4 genuinely different routes, explain the outcome and tradeoff of each in plain language, and recommend one based on the provisional learner profile.

Ask the learner to choose or revise the route. Resolve only dimensions that materially affect the course:

- desired outcome and time horizon;
- how much prerequisite theory is enough;
- which subfields deserve depth and which may be surveyed or skipped;
- desired balance of explanation, original-paper reading, and hands-on practice;
- the form of practice: worked reasoning, data analysis, coding, reproduction, design exercise, experiment planning, or a project;
- whether operational execution belongs in this conversation or elsewhere.

If an important ambiguity remains after the response, ask one concise follow-up. Otherwise, finalize the route. Do not begin formal lessons before this alignment step unless the user explicitly asks to start immediately or has already supplied these choices.

### 4. Select and combine learning modes

Choose the closest mode and adapt it rather than forcing a fixed syllabus:

- **Comprehensive:** build durable, field-wide understanding.
- **Quick start:** reach useful competence through the shortest coherent route.
- **Project-led:** teach prerequisites just before the learner needs them for a real project.
- **Paper-led:** enter the field through a small set of landmark and current papers while filling prerequisite gaps.
- **Refresher:** diagnose weak or outdated areas and rebuild only those.

Read [curriculum-modes.md](references/curriculum-modes.md) when choosing lesson counts, sequencing, or a hybrid mode.

### 5. Verify the evidence map

Build a compact evidence map covering:

1. what the field studies and why it matters;
2. foundational concepts and prerequisite dependencies;
3. historical turning points;
4. current major approaches and representative achievements;
5. applications, open questions, and genuine disagreements;
6. reliable starting sources for later lessons.

Use current web research whenever facts, methods, standards, software, or recent achievements may have changed. Prefer original research, official documentation, authoritative textbooks, and strong reviews. Verify landmark claims and do not invent citations or paper content.

Read [research-and-sources.md](references/research-and-sources.md) when conducting nontrivial research, downloading sources, or organizing a local literature library.

### 6. Design an intentionally uneven curriculum

Organize the course around how understanding grows, not around a list of tools or papers.

Normally begin with:

1. What is this field?
2. What problems does it solve, and why are they difficult?
3. How did the field develop, and what recent results changed its capabilities?
4. What foundational concepts are needed to understand the methods?

Then allocate depth according to the learner's goal. A good course need not treat every unit equally. Compress prerequisites to the smallest coherent foundation, survey secondary areas through their principles and representative achievements, and spend the saved time on the priority area through deeper mechanism, original papers, and practice.

For every unit, specify why it is included, its depth (foundation, survey, working knowledge, or deep study), how papers will be used (mentioned, guided, or closely read), and what practice or independent artifact is expected. Integrate theory, papers, and practice as one progression: teach enough theory to understand a method, reconstruct it through its paper, then use a focused exercise to expose what the learner can and cannot yet do. Practice should serve a conceptual decision, not become generic setup.

Give each lesson one central question. Make every lesson depend naturally on earlier lessons and prepare the next one. Use named tools and models as cases within the conceptual map, not as the map itself.

Present the finalized route and explicitly reflect the learner's choices. Once approved, start or resume the next lesson in the same turn unless they asked only for a plan.

### 7. Teach for understanding

Open each lesson with a concrete question, phenomenon, historical episode, or result. Build intuition before introducing formal terminology. Explain why a concept is needed, derive it through a continuous causal story, then add the standard name, necessary mathematics, and technical detail.

Use complete, fluent sentences and meaningful paragraphs. Prefer one sustained example over many disconnected examples. Translate abstractions into a situation the learner can mentally simulate. Introduce formulas only after explaining the problem they capture, and interpret every important term.

Do not let caution dominate introductory teaching. State the main positive model clearly, then add qualifications where they change understanding. Avoid repetitive constructions such as “not X but Y,” compressed label lists, excessive one-line bullets, premature metrics, and encyclopedic model name-dropping.

Read [teaching-and-interaction.md](references/teaching-and-interaction.md) before drafting a full lesson or adapting to user feedback.

### 8. End every lesson with purposeful questions

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

### 9. Introduce papers and practice at the right time

Use reviews, historical narratives, and selected landmark results early to establish the field. Begin full original-paper reading after the learner understands the problem that motivated the paper.

For paper-led lessons, reconstruct the scientific story before dissecting architecture or metrics:

1. the problem and why it mattered;
2. the previous bottleneck;
3. the authors' key idea;
4. how the method realizes that idea;
5. what experiments changed our beliefs;
6. what remains unresolved.

Critical reading is a later layer of understanding, not the default tone of every introductory paragraph.

For a direction central to the learner's goal, follow major paper lessons with focused practice: establish the theory, closely read a representative paper, reproduce a small inference or design decision, inspect failures, and record what the learner can now do independently. For secondary directions, a theoretical survey and representative results may be sufficient. Do not require practice everywhere for symmetry.

### 10. Maintain learning artifacts when appropriate

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
- Did the learner see meaningful route choices before the syllabus was fixed?
- Does the allocation of theory, papers, and practice reflect the learner's priorities rather than distribute effort evenly?
- Are important recent claims verified and sourced?
- Is the lesson a coherent explanation rather than an outline expanded into bullets?
- Are terms and formulas introduced after intuition?
- Does one main example carry the explanation?
- Is the language natural, complete, and positive in its main argument?
- Are qualifications proportionate to the learner's current stage?
- Do the final questions test explanation, reasoning, and transfer?
- Will the learner's answers meaningfully influence the next lesson?

If several checks fail, revise the lesson before sending it.
