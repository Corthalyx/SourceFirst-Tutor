# SourceFirst Tutor

**Version:** 1.0.2  
**License:** MIT  
**Primary skill file:** [`SKILL.md`](SKILL.md)

SourceFirst Tutor is a universal, source-first AI tutoring skill for learners across subjects, languages, ages, learning levels, and educational systems. It teaches from the learner's own study materials, explains concepts in very simple language, helps replace rote memorisation with understanding, tracks learning progress where supported, and creates practice activities and assessments suited to the learner's context.

Its central principle is simple: **help the learner understand supplied material well enough to explain or apply it in their own words, rather than relying on rote memorisation.**

## Features

- **Source-first learning:** Use learner-provided books, notes, PDFs, images, past papers, typed text, and accessible video/transcript material as the authority. Flag missing, unreadable, conflicting, or unsupported information instead of guessing.
- **Simple Explain:** Explain concepts in very simple, concrete language with short steps and familiar examples. If the learner still does not understand, try a different and simpler explanation.
- **Chapter Clear:** Read all accessible materials for a chapter, unit, or topic; build a source map; teach in an organised sequence; and track what has and has not been covered.
- **Answer Rewrite:** Rewrite supplied study-guide or model answers in clear, natural language while preserving the source's facts, reasoning, terminology, examples, and conclusion.
- **Past-Paper and Question Bank:** Organise supplied past questions using relevant metadata, such as subject, topic, exam or institution, date/year, question type, marks, and source location.
- **Source references:** Provide file/book name, printed page, PDF page where different, and line/paragraph identifiers where available. Never fabricate a locator.
- **Learning Memory Record:** Track study progress, difficult concepts, effective explanations, mistakes, assessment results, and the next starting point when persistent memory or saved records are supported.
- **Adaptive Test Mode:** Build assessments using the learner's requested format, supplied syllabus, sample papers, past papers, rubrics, or course requirements. Do not assume a fixed mark total or one country's examination structure.
- **Fair assessment:** Accept correct ideas expressed in the learner's own words and use transparent marking criteria for open-ended responses.

## Repository Contents

| File | Purpose |
|---|---|
| [`SKILL.md`](SKILL.md) | Main universal skill instructions and required YAML metadata, written in English |
| [`README.md`](README.md) | Project overview and usage guide |
| [`CHANGELOG.md`](CHANGELOG.md) | Version history |
| [`LICENSE`](LICENSE) | MIT License terms |

## How to Use

1. Open [`SKILL.md`](SKILL.md) and review the instructions.
2. Add the skill folder to the supported AI platform's skills directory, or use the platform's documented skill-import workflow.
3. This project uses the standard `SKILL.md` filename and YAML frontmatter with the required `name` and `description` fields. Individual platforms may impose additional requirements, so check the target platform's documentation before installing.
4. Provide the relevant learning materials. Multiple sources can be supplied together, including textbooks, study guides, notes, PDFs, images, typed text, past papers, and accessible video links or transcripts.
5. Ask for the task you want, such as **Simple Explain**, **Chapter Clear**, **Answer Rewrite**, **Add Past Question**, **Test me**, **Objective practice**, **Review my mistakes**, or **Resume topic**.
6. For a topic-based formal assessment, complete the Chapter Clear workflow first. The tutor should ask whether you have questions and whether you are ready before starting.

### Example Requests

- “Explain this idea in the simplest possible way.”
- “Teach me this entire unit using all the files I uploaded.”
- “Rewrite this model answer in easy language without changing its facts or reasoning.”
- “Add these past-paper questions to the question bank.”
- “Create a medium-difficulty assessment using the format in these sample papers.”
- “Give me 15 multiple-choice questions from this topic.”
- “Show the source page and the line where this answer begins.”
- “Resume this topic from my saved Learning Memory Card.”

## Universal and Adaptive Assessment

SourceFirst Tutor does **not** impose a fixed 100-mark paper, question count, question taxonomy, or national examination format. It derives the assessment structure from the learner's instructions, supplied syllabus, sample or past papers, official rubrics, or course requirements. Depending on the context, assessment items may include objective questions, short answers, extended responses, essays, calculations, proofs, case analysis, source interpretation, practical tasks, oral prompts, projects, or other suitable formats.

If no format is available, the tutor should ask a concise clarification or offer an adjustable default blueprint before beginning. It should state the structure, duration, available choices, and scoring before the learner starts. Answers should remain hidden during a live assessment unless immediate feedback is explicitly requested.

After the learner finishes, the tutor provides answer keys, source-based explanations, model responses, and transparent rubrics. Open-ended answers are assessed by the correctness of their ideas and reasoning, not by exact wording.

## Sources, Memory, and Platform Limitations

- The skill does not grant new technical capabilities by itself. Reading PDFs, scanned images, external links, YouTube/Facebook videos, or transcripts depends on the AI platform's available tools and permissions.
- If a source cannot be accessed or read, the tutor must say so and request an accessible file, clearer image, or transcript instead of claiming to have read it.
- A Markdown skill file alone cannot guarantee memory across chats or sessions. For reliable continuity, save the generated **Learning Memory Card** and provide it again when the platform cannot retrieve the earlier record.
- If supplied material cannot support enough valid assessment items, the tutor must disclose the limitation instead of inventing facts to fill the paper.
- For source-based answers, include reliable source locators when available, unless the learner explicitly requests a clean copy without citations.

## Versioning

This repository is at **1.0.2**. See [`CHANGELOG.md`](CHANGELOG.md) for the release history.

## License

This project is distributed under the [MIT License](LICENSE). You may use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the work under the conditions stated in the license. The copyright and permission notice must be included with copies or substantial portions of the work.
