# SourceFirst Tutor

**Version:** 1.0.0  
**License:** MIT  
**Primary skill file:** [`skill.md`](skill.md)

SourceFirst Tutor is a source-locked, understanding-first AI tutor skill for school learning and SSC-style exam preparation. It is designed to teach from the learner’s supplied books, guidebooks, PDFs, scans, images, notes, question papers, typed text, and accessible video or transcript content—rather than silently replacing those materials with outside information.

Its central principle is simple: **help the learner understand the source material well enough to explain it in their own words, instead of relying on rote memorisation.**

## Features

- **Source-locked learning:** Use learner-provided materials as the authority. Flag missing, unreadable, conflicting, or unsupported information instead of guessing.
- **Simple Explain:** Explain concepts in very simple, concrete language, using short steps and familiar examples. If the learner still does not understand, try a different and simpler explanation.
- **Chapter Clear:** Read all accessible materials for a chapter, build a topic/source map, teach the chapter in an organised sequence, and track what has and has not been covered.
- **Answer Rewrite:** Rewrite supplied guide answers in simple, natural, exam-appropriate language while preserving the source’s facts, logic, terminology, examples, and conclusion.
- **Board Question Bank:** Organise supplied board questions by subject, chapter, board, year, question number, and exam part; preserve supplied answers as the basis for accessible-language rewrites.
- **Source references:** Provide file/book name, printed page, PDF page where different, and line/paragraph identifiers when the source makes them available. Never fabricate a locator.
- **Chapter Memory Record:** Track study progress, difficult concepts, effective explanations, mistakes, test results, and the next starting point when the platform supports persistent memory or saved records.
- **Test Mode:** Offer the configured 100-mark model test, optional MCQ practice, answer keys, source-based explanations, marking rubrics, and mistake review.
- **Fair assessment:** Accept correct ideas expressed in the learner’s own words; do not require word-for-word matching with model answers.

## Repository Contents

| File | Purpose |
|---|---|
| [`skill.md`](skill.md) | Main skill instructions, written in English |
| [`README.md`](README.md) | Project overview and usage guide |
| [`CHANGELOG.md`](CHANGELOG.md) | Version history |
| [`LICENSE`](LICENSE) | MIT License terms |

## How to Use

1. Open [`skill.md`](skill.md) and review the instructions.
2. Add the file to the supported AI platform’s skill, custom-instructions, or project-instructions area.
3. Check the target platform’s required file name and format before installing. This repository intentionally uses the lowercase filename `skill.md`; some platforms may require a name such as `SKILL.md` or additional metadata. Rename or adapt the wrapper only when the target platform requires it.
4. Provide the relevant learning material. Multiple sources may be supplied together, including books, guidebooks, notes, PDFs, images, typed text, question papers, and video links or transcripts that the platform can access.
5. Ask for the task you want, such as **Simple Explain**, **Chapter Clear**, **Answer Rewrite**, **Add Board Question**, **Test me**, **MCQ practice**, **Review my mistakes**, or **Resume chapter**.
6. For chapter-based testing, complete the Chapter Clear workflow first. The tutor should ask whether you have questions and whether you are ready before starting the model test.

### Example Requests

- “Explain this idea in the simplest possible way.”
- “Teach me this entire chapter using all the files I uploaded.”
- “Rewrite this guide answer in easy Bangla without changing its facts or reasoning.”
- “Add these past board questions to the question bank.”
- “I am ready for the mid-level chapter test.”
- “Show the source page and the line where this answer begins.”
- “Resume this chapter from my saved Chapter Memory Card.”

## Default Full Model Test

The skill defines the following default structure for a full chapter test:

| Section | Questions | Required answers | Marks |
|---|---:|---:|---:|
| MCQ | 30 | All 30 | 30 |
| Short questions (SQ) | 15 | Any 10 | 20 |
| Creative questions (CQ) | 8 | Any 5 | 50 |
| **Total** |  |  | **100** |

Each creative question is worth 10 marks, divided into the Bengali exam sections: ক = 1, খ = 2, গ = 3, and ঘ = 4. The skill also requires model answers and point-based marking rubrics so answers written in the learner’s own words can be assessed fairly.

The learner can request shorter MCQ practice separately. The full model test must not begin until the chapter has been taught and the learner confirms readiness.

## Sources, Memory, and Platform Limitations

- **The skill does not grant new technical capabilities by itself.** Reading PDFs, scanned images, external links, YouTube/Facebook videos, or transcripts depends on the AI platform’s available tools and permissions.
- If a source cannot be accessed or read, the tutor must say so and request an accessible file, clearer image, or transcript instead of claiming to have read it.
- A Markdown skill file alone cannot guarantee memory across chats or sessions. For reliable continuity, keep the generated **Chapter Memory Card** and provide it again when the platform cannot retrieve the earlier record.
- If source material cannot support the requested number of valid test questions, the tutor must disclose the limitation instead of inventing facts to fill the paper.
- For factual answers based on a supplied source, source locators should be included unless the learner explicitly requests a clean copy without citations.

## Versioning

This repository begins at **1.0.0**. See [`CHANGELOG.md`](CHANGELOG.md) for the release history.

## License

This project is distributed under the [MIT License](LICENSE). You may use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the work under the conditions stated in the license. The copyright and permission notice must be included with copies or substantial portions of the work.
