# Learn from the best — Xavier’s field guide

Six source-based lessons, rewritten for Xavier and other student builders. The exercises and prompts are Toolkit adaptations; the original ideas remain credited below.

Reviewed October 25, 2026. These are selected lessons, not exhaustive summaries of every linked resource.

## Start with a real problem

Explorer · Hands-on course

Source: [Datawhale / easy-vibe](https://github.com/datawhalechina/easy-vibe)

A useful first project begins with someone’s need, then grows through small prototypes and feedback.

- Talk to a potential user before choosing features. Ask about a real task they struggled with.
- Build a small version you can show; use feedback to decide what to improve.
- Learn fundamentals when you need them. Move from prototypes to backend and advanced tools as the project demands.

### Try it, Xavier

Ask a teammate how they remember practice goals. Sketch one screen for their hardest step, then have them try it using sample data.

**Finish with:** One user need, one working interaction, and one change based on feedback.

### Adaptable prompt

Coach me through a small project for [user] who struggles with [task]. Ask about their last real experience. Help me choose one interaction to prototype, a simple test, and a question for user feedback. Let me make the final choice.

## Give AI a map of your project

Builder · AI coding roadmap

Source: [automata / aicodeguide](https://github.com/automata/aicodeguide)

Clear requirements, small tasks, and useful project context make AI coding easier to review.

- Turn a conversation about your idea into a written specification: who it serves and how it should work.
- Break the work into tasks with dependencies, so each step has what it needs.
- Keep run commands, test instructions, and project conventions in an agent-readable guide; review generated code.

### Try it, Xavier

For a club website, write a short brief and three ordered tasks. Explain which task must finish first and why.

**Finish with:** A brief, a task checklist, and instructions another person can use to run the project.

### Adaptable prompt

Read my brief: [brief]. Identify missing information, then make a small ordered task list with a check for each task. Draft project instructions using only commands and facts I provide. Mark anything unknown. Explain the first task before writing code.

## Choose tools for the task

Explorer · Curated directory

Source: [filipecalegario / Awesome Vibe Coding](https://github.com/filipecalegario/awesome-vibe-coding)

Use a tool directory to discover options. A listing is a starting point for evaluation, not proof that a tool fits your project.

- The directory groups browser builders, editors, command-line tools, documentation tools, and communities.
- These categories support different ways of working; start with the task you need to complete.
- Toolkit recommendation: compare a small shortlist using current official information and the same tiny experiment.

### Try it, Xavier

Choose two tools for a one-page club announcement. Compare setup, cost, code export, and data handling before trying either.

**Finish with:** A short comparison and a reason for choosing one option, with unknowns clearly marked.

### Adaptable prompt

Help me compare [tool A] and [tool B] for [small task]. Use current official sources for cost, setup, export and data handling. Separate verified facts from unknowns. Propose the same small test for both. Do not sign me up or install anything.

## Turn an idea into a buildable plan

Builder · Planning workflow

Source: [KhazP / Vibe Coding Prompt Template](https://github.com/KhazP/vibe-coding-prompt-template)

Separate research, product requirements, technical choices, and implementation instructions instead of asking for an entire app at once.

- Research the problem and alternatives before committing to a solution.
- Describe the minimum useful product, then choose technology that supports those requirements.
- Save each planning document so the next stage starts with agreed context.

### Try it, Xavier

Plan a student event signup prototype using fictional attendees. Limit the first version to three features and list what you are leaving out.

**Finish with:** A short problem brief, three must-have features, a technical choice with tradeoffs, and a first-step test.

### Adaptable prompt

My idea is [idea] for [audience]. Guide me through research questions, a one-page product brief, technical options, and a first implementation task. Keep the first version to three features. Ask me to review each stage before continuing; do not invent research findings.

## Keep control as the project grows

Builder · Workflow guide by Nicolas Zullo

Source: [EnzeD / vibe-coding](https://github.com/EnzeD/vibe-coding)

A reviewed plan, small implementation steps, and saved progress help you keep control across AI coding sessions.

- Keep your design goals and technology decisions in project documents.
- Work through focused steps and test them before treating them as complete.
- Record progress and save working versions so a new session can continue from evidence.

### Try it, Xavier

Add one feature to a practice-goal tracker. Record the expected behavior, actual test result, and next step before ending the session.

**Finish with:** One tested change, a saved working version, and a short handoff note.

### Adaptable prompt

Read [project brief] and [progress note]. Confirm the next small task, make only that change, and give me a reproducible test. Report what was actually checked and what remains uncertain. Draft a handoff note with changed files, results, and the next step.

## Turn a repeatable task into a skill

Innovator · Skill examples · repository deprecated

Source: [OpenAI / Skills](https://github.com/openai/skills)

Package a useful workflow as clear reusable instructions, with supporting files only when needed.

- A skill groups instructions and optional scripts or resources around a specific task.
- Toolkit recommendation: state when to use it, what input it needs, the steps, and what a good result looks like.
- The original catalog is deprecated. Follow its links to OpenAI Plugins and current plugin-building guidance for new installations.

### Try it, Xavier

Draft a “student project demo coach” skill. Try it on two different projects and revise any instruction that produces vague results.

**Finish with:** A reusable instruction file and two recorded trials, with original sources credited.

### Adaptable prompt

Help me draft a reusable skill for [repeatable task]. Include when to use it, required inputs, steps, output format, and success checks. Ask about missing details. Test the instructions on two examples I supply, then suggest one focused improvement.

[Current OpenAI plugin examples](https://github.com/openai/plugins)

[Current plugin-building guidance](https://developers.openai.com/plugins/build/plugins)
