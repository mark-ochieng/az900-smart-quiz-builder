# Smart Quiz Builder: AZ-900 Practice (Unofficial)

> **Unofficial study tool.** Not affiliated with or endorsed by Microsoft. All questions are original and written for learning. No Microsoft logos are used.

Built for the **Vibe Coding Hackathon: AZ-900 Exam Prep Edition** (#1MillionDevs, Power Learn Project) in the **Practice & Assessment: Smart Quiz Builder** challenge.

**Live demo:** https://claude.ai/artifact/81xeFMAvdwx4GaSW8MyMRU

**live demo video :** https://drive.google.com/file/d/1w9x2skkfX0x6_RmZZ1c4v6uXS5AsZzZq/view?usp=drivesdk

## The problem

Many learners practise with questions but never understand *why* an answer is right or wrong. They memorise answers and then stumble when the wording changes.

## The solution

A mobile-first quiz app that gives an **instant explanation after every answer**, organised by AZ-900 topic, and shows learners where they are weak.

## Features

- 48 original practice questions across the three AZ-900 areas: Cloud Concepts, Azure Architecture & Services, and Management & Governance.
- Choose a topic and a quiz length of 5, 10 or 20 questions.
- Instant right/wrong feedback with a short explanation for every question.
- Answer order is shuffled every round, so learners cannot memorise positions.
- Results screen with score, breakdown by topic, and a review of every mistake.
- **Retry only my missed questions** mode.
- **Readiness tracker** that builds up accuracy per topic across sessions (saved on the device).
- Light and dark mode, works on phones.

## How to use

1. Open the demo link, or open `index.html` in any browser.
2. Pick a topic and quiz length, then tap **Start quiz**.
3. Tap an answer, read the explanation, then tap **Next question**.
4. At the end, review mistakes or retry only the questions you missed.

## Tech

Single-file HTML, CSS and vanilla JavaScript with no dependencies. Progress is stored in the browser's `localStorage`. The question bank is a plain array, so topics and certifications are easy to add.

## Tools and process

Built with **Claude** for prompt engineering, question writing and code generation. See [PROMPT_LOG.md](PROMPT_LOG.md) for the prompts used and why.

## Scaling to other certifications

Each question is `[topic, question, options, correctIndex, explanation]`. Replacing the bank and the topic names gives a quiz for AI-900, AZ-104, or other certifications. A Supabase backend could later add accounts, shared leaderboards and cohort analytics.

## Content and accuracy

Content follows the public AZ-900 skills outline on Microsoft Learn. Questions are original, not copied from any exam. Always verify against the official Microsoft Learn material before sitting the exam.

## Author

Mark Ochieng.
