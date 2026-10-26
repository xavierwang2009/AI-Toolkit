# Xavier's AI Toolkit

Empowering young creators with curated AI skills, prompts, coding tools, and hands-on projects to turn ideas into real-world solutions.

Website: https://xavier-ai-toolkit.lx2rice.chatgpt.site

## Source files

- `dist/`: complete PWA source, including HTML, CSS and JavaScript, icons, app manifest and offline service worker.
- `skills/`: all 10 skill instructions, copied verbatim from the website.
- `projects/`: all 3 project challenge guides, copied verbatim from the website.
- `.openai/hosting.json`: existing ChatGPT Sites hosting configuration.

## Run locally

No dependencies or build step are required.

```sh
python3 -m http.server 8000 --directory dist
```

Open http://localhost:8000. Serve `dist` at the domain root; the app uses root-relative URLs. GitHub commits do not automatically deploy to the existing ChatGPT Site.

## Skills

- [Idea Explorer](skills/idea/SKILL.md) — Explorer
- [Prompt Improver](skills/prompt/SKILL.md) — Explorer
- [Project Planner](skills/plan/SKILL.md) — Explorer
- [UI Design Coach](skills/design/SKILL.md) — Builder
- [Website Starter](skills/web/SKILL.md) — Builder
- [App MVP Builder](skills/app/SKILL.md) — Builder
- [Code Explainer](skills/explain/SKILL.md) — Explorer
- [Debugging Coach](skills/debug/SKILL.md) — Builder
- [Project Reviewer](skills/review/SKILL.md) — Innovator
- [Launch & Demo Coach](skills/launch/SKILL.md) — Innovator

## Project guides

- [My First Mini Game](projects/game/GUIDE.md)
- [My Passion Website](projects/website/GUIDE.md)
- [My Everyday Helper](projects/app/GUIDE.md)

## Attribution and maintenance

The website retains links to original learning resources from Datawhale, automata, filipecalegario, KhazP, EnzeD and OpenAI. These external repositories and skill collections are not bundled here; their materials belong to their respective creators.

The Markdown instructions mirror the prompts in `dist/data.js`. Keep both in sync when editing.

## Source-based learning guide

[Learn from the best](LEARNING-GUIDE.md) contains six rewritten lessons, practical exercises, and reusable prompts with source attribution. The same lessons are available in the website’s Resources section and cached with the PWA. [Research notes](RESOURCE-NOTES.md) record the reviewed sources.

## Interactive workspace

Home offers three starting choices. Skills provides search, level filters and prompt copying. Projects presents a brief, planning prompt and test guide. Lessons separates key ideas, exercises and prompts. Navigation uses URL fragments, supports browser Back, and changes to a bottom bar on mobile. Motion can be disabled with the toolbar control and respects reduced-motion preferences.

- `dist/data.js`: the 10 original skills, 3 project challenges and 6 attributed lessons.
- `dist/app.js`: navigation, filters, copy controls, installation and updates.
- `dist/style.css`: responsive workspace and motion.
