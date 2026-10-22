# Prompt Log: Smart Quiz Builder (Unofficial AZ-900 Practice)

This log shows how prompts were designed and why. Each follows the same pattern: **role, goal, constraints, output format**.

## Prompt 1: Build the first version

**Prompt**
> You are a front-end developer and Azure trainer. Build a mobile-first, single-file HTML quiz app for AZ-900 practice. Requirements: original questions only (never copy exam questions), organised into three topics (Cloud Concepts, Architecture & Services, Management & Governance), instant feedback with a one-sentence explanation after every answer, score summary by topic, light and dark mode, and an "Unofficial study tool" banner with no Microsoft logos.

**Why it works**
- Role plus audience sets both the technical and teaching quality.
- The "original questions only" constraint follows the hackathon rules.
- Output format (single file, mobile-first) makes it easy to share and test on a phone.

## Prompt 2: Question writing

**Prompt**
> Write original AZ-900 practice questions based on the public skills outline. For each: four options with one correct answer, plausible distractors that reflect real misconceptions, and a one-sentence explanation of why the answer is correct. Cover each topic evenly and use plain language.

**Why it works**
- Plausible distractors force learners to think instead of guess.
- Explanations directly address the problem statement: learners not knowing *why*.
- Even topic coverage supports the readiness score.

## Prompt 3: Upgrade for learning value

**Prompt**
> Expand the question bank to about 48 questions. Add a "retry only my missed questions" mode and a readiness tracker that stores accuracy per topic across sessions. Keep the code dependency-free and edit only what changes.

**Why it works**
- Targets weak spots, which is where learning gains come from.
- A narrow edit instruction keeps the code stable and reduces regressions.

## Prompt 4: Quality check

**Prompt**
> Review each question for factual accuracy against the public AZ-900 skills outline. Flag ambiguous wording, answers that give hints, and distractors that could also be correct.

**Why it works**
- Judges score accuracy of content, so a separate review pass lowers the risk of errors.

## Prompt 5: Documentation and pitch

**Prompt**
> Write a README and a 6-slide pitch outline for the Smart Quiz Builder. Match the pitch scoring: problem, solution demo, target users, impact and scalability, clarity.

**Why it works**
- Structure follows the judges' rubric, so each section earns marks.

## Lessons learned

- Specific constraints produce better output than long descriptions.
- Ask for original content explicitly to stay within the hackathon rules.
- Small, focused edit prompts beat full rewrites.
- Always test on a phone and verify facts against Microsoft Learn.
