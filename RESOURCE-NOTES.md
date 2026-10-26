# Learn from the best — notes for Xavier

Reviewed: 2026-10-25. These are original, AI-assisted summaries of the linked authors' work, adapted for Xavier's learning. They are not Xavier's original methods or evidence that he has completed these exercises. Suggested applications below are our adaptations, not upstream claims.

## 1. Easy-Vibe — start with a real person and a small problem

**Source:** [Datawhale's Easy-Vibe](https://github.com/datawhalechina/easy-vibe). **Type:** Hands-on course, with beginner projects, full-stack development, and advanced workflows.

- Choose a problem by asking how people handle it today, where that process fails, and how often it matters. A novel feature is not proof of a need.
- Follow a learning path that matches the next outcome: first prototype, complete application, or advanced workflow. Learn missing fundamentals when they become relevant.
- Try the entire user journey, observe someone else attempting it, and repair the main blockers before adding features. Test failure and missing-input cases too.

**Try this, Xavier:** Ask a teammate how they review practice footage. Build one small aid for a specific difficulty, then watch them use it without coaching them through the interface. Record one observation and the change it led to. For a school or service project, usefulness can matter more than willingness to pay.

**Read next:** [Finding Great Ideas](https://datawhalechina.github.io/easy-vibe/en/stage-1/finding-great-idea/) · [Complete Project Practice](https://datawhalechina.github.io/easy-vibe/en/stage-1/complete-project-practice/).

## 2. AI Code Guide — give AI a clear brief and check its work

**Source:** [automata/aicodeguide](https://github.com/automata/aicodeguide). **Type:** Practical roadmap and workflow guide.

- Describe the intended user, requirements, and constraints before requesting code. Use a question-and-answer conversation to expose missing decisions.
- Save the brief and break the work into connected tasks. Keep project instructions, setup steps, and verification commands in `AGENTS.md` so later sessions have context.
- Review and test generated work. AI agreement and confident explanations do not transfer responsibility away from the person building the project.

**Try this, Xavier:** For the next toolkit feature, write the audience, desired behavior, and a check that would prove it works. Ask AI to explain unfamiliar code, then explain the important decision back in your own words. Save the test result alongside the task.

**Read next:** [Prompting and project workflow](https://github.com/automata/aicodeguide#how-i-prompt-for-coding-aka-how-i-vibe-code).

## 3. Awesome Vibe Coding — use a directory to find a suitable tool

**Source:** [Filipe Calegario's Awesome Vibe Coding](https://github.com/filipecalegario/awesome-vibe-coding). **Type:** Curated resource directory, not a step-by-step course or independent performance ranking.

- The list separates browser builders, editors, command-line tools, and other interfaces. These categories help narrow a search to the way you want to work.
- It also lists task-management and documentation resources: organizing work and supplying context are separate needs from generating code.
- Its links lead to individual projects and documentation. Inclusion in the list is a starting point for investigation, not proof that a tool suits your project.

**Try this, Xavier:** Start with one task and compare at most two tools on that same task. Record whether you could understand, edit, test, and export the result. Check current pricing and data handling at each tool's own site before choosing. This comparison method is our suggested exercise.

**Read next:** [Tool categories](https://github.com/filipecalegario/awesome-vibe-coding#contents) · [Documentation resources](https://github.com/filipecalegario/awesome-vibe-coding#documentation-for-ai-coding).

## 4. Vibe Coding Prompt Template — turn research into a bounded first version

**Source:** [KhazP/vibe-coding-prompt-template](https://github.com/KhazP/vibe-coding-prompt-template). **Type:** Planning prompts and document workflow.

- Move through research, product requirements, technical design, and coding-assistant instructions. Carry saved decisions into each next step.
- Separate required features from what can wait. Give each required feature observable success criteria; do not add accounts, databases, or AI merely because a template mentions them.
- Keep unknowns visible. A generated research request is not research evidence, and unsupported claims should remain labeled as assumptions.

**Try this, Xavier:** Make a one-page brief for a student tool: who it serves, one problem, the smallest useful result, what is excluded, and how you will test it. Ask AI to identify missing decisions before implementing the first feature.

**Read next:** [MVP requirements prompt](https://github.com/KhazP/vibe-coding-prompt-template/blob/main/part2-prd-mvp.md) · [Agent handoff prompt](https://github.com/KhazP/vibe-coding-prompt-template/blob/main/part4-notes-for-agent.md).

## 5. EnzeD's Vibe Coding Guide — build, check, and save one step at a time

**Source:** [Nicolas Zullo's guide in EnzeD/vibe-coding](https://github.com/EnzeD/vibe-coding). **Type:** Opinionated implementation workflow, illustrated with games.

- Review the design and choose a simple technical approach before building. Keep the base project small enough to finish.
- Give each implementation step a specific check, and validate that step before moving to the next.
- Save working milestones in Git and keep progress and architecture notes current so a fresh chat can resume accurately.

**Try this, Xavier:** Make one change, run its check, and save the working version. Add a short note: what changed, what you tested, and what remains uncertain. Keep the note useful enough that tomorrow's session can continue without guessing.

**Read next:** [Implementation plan and memory bank](https://github.com/EnzeD/vibe-coding#3-implementation-plan) · [Build workflow](https://github.com/EnzeD/vibe-coding#workflow).

The durable lesson is the workflow. The guide's preferred models and product rankings are the author's time-sensitive opinions, not requirements for Xavier.

## 6. OpenAI Skills — make a repeatable task into reusable instructions

**Source:** [openai/skills](https://github.com/openai/skills). **Type:** Official skills catalog and examples; the repository currently marks itself deprecated and directs readers to [openai/plugins](https://github.com/openai/plugins).

- A skill packages instructions and, when useful, supporting scripts or resources for a particular repeatable task.
- Reusable instructions belong in a discoverable package. Current plugin guidance shows a `SKILL.md` containing a name, description, and task instructions.
- Check the license attached to an individual skill before reusing its contents; the old catalog points to licenses inside skill directories.

**Try this, Xavier:** Pick a task you have already done more than once, such as checking a project demo. Write its inputs, steps, expected output, and checks in plain language. Test the instructions on another example, then revise the unclear parts. Credit any source whose instructions you adapt.

**Current guidance:** [Build a plugin, including a minimal skill](https://developers.openai.com/plugins/build/plugins). These toolkit notes are reading material; a saved Markdown page alone does not demonstrate that a skill has been installed or tested in an agent.

## A short practice loop

This is our synthesis for Xavier:

1. Find one real problem and ask how someone handles it now.
2. Write the smallest useful outcome and a check for success.
3. Give AI the relevant context and build one manageable step.
4. Read the important code, run the check, and try the whole user journey.
5. Record feedback, save the working version, and explain what you learned.
6. Turn a proven repeated task into a reusable instruction only when it helps.

Keep a student development log that distinguishes your decisions and code from AI assistance and reused material. A working demo, an explanation you understand, and an honest account of limitations are stronger evidence than a long feature list.
