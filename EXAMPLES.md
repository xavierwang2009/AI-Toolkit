# Complete prompt examples

These are illustrative student scenarios, not claims about completed work. Each prompt can be copied as written or adapted.

## Skills

### Idea Explorer

```text
Act as a friendly project mentor for a middle/high school student. I care about helping young swimmers remember their equipment before practice. I am a ninth-grade student with basic HTML experience and one weekend to build a prototype. Ask me three clarifying questions one at a time, then suggest three achievable digital project ideas. For each, explain who it helps, a simple first version, what I would learn, and a realistic challenge. Do not choose for me.
```

### Prompt Improver

```text
Improve this prompt for an AI assistant: Make me a packing app for swimming practice. I want it to remember my list on my phone, but I have never used a database. I have two afternoons and know a little HTML. First identify missing context, then ask up to three key questions. Give me an improved prompt with role, goal, background, constraints, desired output and a way to check success. Explain what changed in plain English.
```

### Project Planner

```text
I want to build a swimming-practice packing checklist for students who forget their equipment. My experience level is beginner with basic HTML knowledge. Create a one-page project brief: problem, target users, three essential features, non-goals, technology options with pros/cons, milestones, tests and completion checklist. Challenge unrealistic assumptions. Keep version one doable in six hours over one weekend. Ask before coding.
```

### UI Design Coach

```text
Act as a UI/UX mentor. Design a simple, accessible packing-checklist web app for student swimmers using phones that helps them add equipment, mark it packed, and reset their list before each practice. First describe the main user journey, then a screen-by-screen layout, navigation, typography, colors, empty states, mobile behavior and usability checks. Give two distinct visual directions and explain tradeoffs. Do not write code yet.
```

### Website Starter

```text
Help me build a responsive website for a beginner-friendly swimming club information page using HTML, CSS and JavaScript. I am a beginner who understands HTML tags but has not written JavaScript. It should include an introduction, a sample weekly practice schedule, an equipment checklist, and a frequently asked questions section and support expandable FAQ answers and equipment checkboxes. Use clearly labeled sample schedules and no personal photos or real contact details. Start with a simple file plan, then implement the smallest working version. Explain each file. Include keyboard/mobile usability and tell me exactly how to run and test it locally. Avoid unnecessary dependencies.
```

### App MVP Builder

```text
You are my coding coach. Here is my project brief: Practice Pack: a browser-local packing checklist for a student swimmer. Features: add an item, mark it packed, and reset all checkboxes for the next practice. Use HTML, CSS and JavaScript, with localStorage on this device. No accounts, uploads, or personal information. I know basic HTML and have one weekend. Done means items survive refresh, empty items are rejected, and all controls work with a keyboard.. Help me create an MVP with only the three must-have features. Propose the simplest reasonable tech stack and explain its tradeoffs. Break the build into testable steps. Implement step one only and wait for my test results before proceeding. Never assume a feature works without evidence.
```

### Code Explainer

```text
Explain this code to me as a ninth-grade student: function remaining(items) { return items.filter(item => !item.packed).length; }
const kit = [{ name: "Goggles", packed: true }, { name: "Towel", packed: false }];
console.log(remaining(kit));. Start with what it does overall, then walk through the important parts using a simple analogy. Point out the inputs, outputs and likely failure cases. Ask me two short comprehension questions and suggest one safe change I can try myself.
```

### Debugging Coach

```text
Help me debug a problem without making unrelated changes. Expected behavior: Clicking Add should append Goggles to the visible list without reloading the page. Actual behavior: the list stays empty and the console reports an error. Steps to reproduce: Save the following complete snippet as index.html, open it, open the browser console, and click Add. Exact error/output: Uncaught TypeError: Cannot read properties of null (reading 'appendChild'). Relevant code: <button id="add">Add</button><ul id="items"></ul><script>document.getElementById("add").onclick=()=>{const li=document.createElement("li");li.textContent="Goggles";document.getElementById("item-list").appendChild(li);};</script>. Give the most likely causes, the smallest diagnostic test, then one focused fix. Explain why it works and how to verify it. If information is missing, ask first.
```

### Project Reviewer

```text
Review my packing-checklist website for a student project. Goal: help students track equipment for a practice session. Features: type an item, add it to a list, and mark it packed. This prototype does not save data yet. Code or screenshots: <!doctype html><html lang="en"><meta charset="utf-8"><meta name="viewport" content="width=device-width, initial-scale=1"><title>Practice Pack</title><h1>Practice Pack</h1><form id="form"><label for="item">New item</label><input id="item"><button>Add</button></form><ul id="list"></ul><script>document.getElementById("form").onsubmit=e=>{e.preventDefault();const input=document.getElementById("item");const li=document.createElement("li");const label=document.createElement("label");const box=document.createElement("input");box.type="checkbox";label.append(box,document.createTextNode(input.value));li.append(label);document.getElementById("list").append(li);input.value="";};</script></html>. Assess functionality, ease of use, mobile behavior, accessibility, privacy and security basics, and edge cases. Prioritize findings as critical/important/nice-to-have. Give reproducible tests and recommend the three highest-impact improvements. Distinguish verified issues from guesses.
```

### Launch & Demo Coach

```text
Help me prepare Practice Pack, a browser-local equipment checklist with add, check-off, and reset controls for a responsible launch and two-minute demo. Audience: classmates and a teacher. This is a sample demo scenario; ask me what I personally wrote, how AI helped, and which tests actually passed before drafting those claims. Create a pre-launch checklist for testing, privacy, permissions, attribution, dependency/security checks, and rollback. Then outline a demo: problem, motivation, live workflow, what I personally built, how AI helped, limitations and next steps. Do not invent test results or impact.
```

## Projects

### My First Mini Game

```text
Coach me to create a very simple browser game about catching falling swim goggles with a basket. Move the basket with arrow keys or on-screen left/right buttons. Catch ten goggles to win; miss three to lose. Each catch scores one point and Restart resets the score and misses. I am a beginner. Keep it to one HTML file initially. Start with the game rules and acceptance checklist. Then give runnable code and explain how I can test winning, losing, score and restart. Suggest one optional personalized feature after it works.
```

### My Passion Website

```text
Help me plan and build a responsive website about a fictional school swimming club called Blue Wave. Use clearly labeled sample information instead of real meeting details. Audience: students who are curious about joining and want to know what to bring to their first practice. Include a homepage introduction, three useful sections, and one working interaction. Ask about my content, propose a clean layout, then build a minimal version in HTML/CSS/JS. Provide a testing checklist and deployment options.
```

### My Everyday Helper

```text
I want to make a small useful app that helps a student swimmer with forgetting goggles, a towel, or a water bottle before practice. The student needs to reuse a packing list, check items off, and reset it for the next session without making an account. Interview me to understand the workflow. Create a short project brief with three essential features, a minimal data model, privacy considerations and test cases. Then guide me through building one feature at a time. Start with a browser-local prototype if suitable.
```

## Lessons

### Start with a real problem

```text
Coach me through a small project for a student swimmer who struggles with packing their bag before after-school practice. This is a sample user scenario, not an interview result; ask me to collect a real example before drawing conclusions. Ask about their last real experience. Help me choose one interaction to prototype, a simple test, and a question for user feedback. Let me make the final choice.
```

### Give AI a map of your project

```text
Read my brief: Practice Pack: a browser-local packing checklist for a student swimmer. Features: add an item, mark it packed, and reset all checkboxes for the next practice. Use HTML, CSS and JavaScript, with localStorage on this device. No accounts, uploads, or personal information. I know basic HTML and have one weekend. Done means items survive refresh, empty items are rejected, and all controls work with a keyboard. Files: index.html, style.css, app.js. Run by opening index.html in a browser. There is no package manager or automated test command yet. Do not invent one.. Identify missing information, then make a small ordered task list with a check for each task. Draft project instructions using only commands and facts I provide. Mark anything unknown. Explain the first task before writing code.
```

### Choose tools for the task

```text
Help me compare plain HTML/CSS/JavaScript and React with Vite for a single-screen equipment checklist that runs in the browser and stores data locally; I am a beginner and have six hours. Use current official sources for cost, setup, export and data handling. Separate verified facts from unknowns. Propose the same small test for both. Do not sign me up or install anything.
```

### Turn an idea into a buildable plan

```text
My idea is a reusable equipment packing checklist for student swimmers who pack in a hurry. I have no user research yet, know basic HTML, and can spend six hours on a prototype. Guide me through research questions, a one-page product brief, technical options, and a first implementation task. Keep the first version to three features. Ask me to review each stage before continuing; do not invent research findings.
```

### Keep control as the project grows

```text
Read Practice Pack: a browser-local packing checklist for a student swimmer. Features: add an item, mark it packed, and reset all checkboxes for the next practice. Use HTML, CSS and JavaScript, with localStorage on this device. No accounts, uploads, or personal information. I know basic HTML and have one weekend. Done means items survive refresh, empty items are rejected, and all controls work with a keyboard. and Sample handoff: index.html has an accessible form and list; app.js adds items as text and toggles checkboxes. Manual checks recorded for this fictional scenario: adding Goggles and checking it worked. Empty input still adds a blank row. Refresh persistence is not implemented. Next task: trim input and reject blank items only. Ask me for the actual files before changing code; the sample handoff is not proof about a real repository.. Confirm the next small task, make only that change, and give me a reproducible test. Report what was actually checked and what remains uncertain. Draft a handoff note with changed files, results, and the next step.
```

### Turn a repeatable task into a skill

```text
Help me draft a reusable skill for turning a teacher-provided assignment into a student work checklist, without doing the assignment. Inputs are the assignment text, due date, available study time, and required deliverables. Use these two sample inputs: (1) Write a 600-word comparison of two class readings, due Friday, with three quotations; I have 30 minutes daily Monday through Thursday. (2) Prepare a three-minute science presentation about evaporation, due next Wednesday, with one diagram and two sources; I have 45 minutes Saturday and Tuesday. Keep quotations and sources as tasks to find and verify, not invented content. Include when to use it, required inputs, steps, output format, and success checks. Ask about missing details. Test the instructions on two examples I supply, then suggest one focused improvement.
```
