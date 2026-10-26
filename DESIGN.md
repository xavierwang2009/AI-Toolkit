---
name: "Xavier’s AI Toolkit"
description: "A focused student workspace for AI skills, projects, and lessons."
colors:
  coral: "#d9573b"
  ink: "#123d3a"
  muted: "#596861"
  paper: "#faf8f2"
  white: "#ffffff"
  line: "#dce3da"
  accent: "#b5412c"
  tint: "#e5f3ec"
  mint: "#d7f3e5"
  selected: "#d7f3e5"
  starter: "#d7f3e5"
  focus: "#b5412c"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "clamp(36px, 4.5vw, 66px)"
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: "-.04em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "32px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-.035em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "28px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-.035em"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: "normal"
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", sans-serif"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: normal
    letterSpacing: "normal"
rounded:
  quiet: "8px"
  control: "10px"
  prompt: "12px"
  detail: "16px"
  pill: "20px"
  starter: "24px"
spacing:
  small: "8px"
  compact: "12px"
  medium: "16px"
  inset: "20px"
  large: "24px"
  detail: "30px"
  section: "32px"
  workspace: "36px"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.white}"
    rounded: "{rounded.control}"
    padding: "14px 19px"
  button-secondary:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    padding: "10px 14px"
  button-quiet:
    textColor: "{colors.ink}"
    rounded: "{rounded.quiet}"
    padding: "8px 11px"
  input-search:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "12px 14px"
  chip-level:
    backgroundColor: "{colors.tint}"
    rounded: "{rounded.pill}"
    padding: "6px 10px"
  detail-panel:
    backgroundColor: "{colors.white}"
    rounded: "{rounded.detail}"
    padding: "30px"
  navigation:
    rounded: "{rounded.control}"
    padding: "14px 16px"
---

# Design System: Xavier’s AI Toolkit

## Overview

**Creative North Star: "The Focused Workspace"**

The focused workspace uses deep teal for orientation, mint for selection and guided starting points, and mint for small identity and learning cues. Its character is calm, direct, and practical: clear controls surround a generous working surface.

System UI typography is intentional for Operate mode, with Read behavior inside lessons. Color, borders, and spacing establish hierarchy without decorative elevation. The implementation uses inline SVG interface icons; existing PNG app icons predate this task and remain unchanged. No generated raster imagery shipped in this redesign.

**Key Characteristics:**

- Persistent navigation and visible selection.
- Flat surfaces with tonal separation.
- Readable instructions and source attribution.
- Brief motion with an explicit off control.

## Colors

Navy anchors the interface; pale mint and mint soften the working environment without competing with the content. The frontmatter records the implemented values.

### Primary
- **Deep Teal** (`ink`): navigation rail, main text, selected intent, active filters, and primary actions.
- **Coral Text** (`purple`): headline emphasis, active lesson tabs, and hover emphasis.

### Secondary
- **Mint Wash** (`tint`): level badges and mobile navigation selection.
- **Selected Mint** (`selected`): the current collection item.
- **Starter Mint** (`starter`): the live suggested-next-move surface.

### Tertiary
- **Soft Mint** (`mint`): the initial mark. Related green surfaces identify Explorer levels and practical exercises.

### Neutral
- **Warm Cream** (`paper`): application background and prompt blocks.
- **Working White** (`white`): reading/detail surfaces and active desktop navigation.
- **Slate Text** (`muted`): supporting copy and metadata.
- **Soft Divider** (`line`): input borders, panel outlines, and separators.
- **Focus Coral** (`focus`): keyboard focus outlines.

## Typography

**Display Font:** system UI, using the frontmatter stack.
**Body Font:** the same system UI stack; prompts also use this family.

**Character:** Familiar operating-system typography keeps controls immediately legible and lessons readable. The large Home heading supplies emphasis; there is no decorative display-family dependency.

### Hierarchy
- **Display:** Home question, responsive on desktop; fixed to 38px on phones.
- **Headline:** workspace heading; 28px on phones.
- **Title:** detail heading; 25px on phones. Starter heading is 27px, becoming 23px on phones.
- **Body:** descriptive paragraphs; detail descriptions become 14px on phones. Reading blocks use approximately 66–75ch maximum measures, with 1.65–1.8 line height depending on content.
- **Label:** compact counts, levels, supporting navigation text, and source metadata. Main navigation uses 15px at weight 600; mobile navigation uses 12px.

## Layout

At a 1280px desktop viewport, a 212px left rail sits beside the workspace. A 78px top bar precedes the scrollable main region, whose padding is 32px vertically and 36px horizontally. Views cap at 1300px; Home caps at 1200px. The Home starter and intent choices sit side by side.

Collection views use a 290px list alongside a flexible white detail panel, separated by 24px. At widths of at least 1100px, list and detail panels can scroll independently within a workbench height of `calc(100dvh - 252px)`. At or below 1100px, the rail becomes 180px, list becomes 240px, and the gap becomes 16px; the overlapping 1100px boundary follows normal CSS cascade order.

At or below 760px, navigation becomes a fixed four-item bottom bar with safe-area padding. The top bar becomes 60px; the workspace reserves 65px plus the safe-area inset below. Home stacks its starter below three compact intent buttons; its introductory strip and desktop destination links are hidden. Collection views show the list first, then show the detail after selection; an “All” back control returns to the list.

The current content inventory is 10 skills, 3 projects, and 6 attributed lessons. Those counts describe this implementation, not a permanent visual-system constraint. Search and experience filters remain beside the desktop detail panel. Skill progression stays within the currently matching results.

## Elevation & Depth

There are no box shadows in the current system. White detail panels, mint selections, navy controls, and fine borders separate layers. Toasts sit above the workspace through positioning, not a shadow treatment.

## Shapes

Controls use compact rounded rectangles; prompt blocks are slightly softer and detail panels larger. The Home starter has the largest corner treatment, reduced to the detail radius on phones. Level badges are pill shaped, while the starter symbol and avatar are circles. Borders are generally one pixel; keyboard focus uses a three-pixel outline with a four-pixel offset.

## Components

### Buttons

Direct, legible controls. Primary buttons use navy with white text and darken to a lighter navy on hover. Secondary buttons are white with a fine divider border and a 9px radius. Quiet top-bar controls are transparent with a divider border. Disabled controls use 45% opacity and a default cursor. Interactive controls share the violet focus outline.

### Chips

Level badges are descriptive: Builder uses mint, Explorer green, and Innovator amber. Experience filters are buttons with a navy selected state and `aria-pressed`; inactive filters remain transparent. These have distinct roles even where their compact shapes are similar.

### Cards / Containers

Detail panels use white, a fine border, and generous internal padding. Prompt blocks use Warm Cream with preserved line breaks. Green exercise boxes separate concrete tasks from lesson explanation. No hover lift is applied to these reading surfaces.

### Inputs / Fields

Search uses a white background, divider border, rounded corners, and purple caret. Its visible label names the collection. No error-state design is implemented; empty results display an explanatory message in both collection and detail areas.

### Navigation

Desktop links use subdued blue-white text on navy, with white active backgrounds and navy active text. Mobile links stack icon and label on white; mint identifies the active destination. Current pages use `aria-current`. Collection items use mint selection, a subtle outline, and `aria-pressed`. Lessons and project steps use a purple underline for the active segment.

### Suggested Next Move

Three intent buttons update a mint preview with a title, concise explanation, three-step sequence, and a direct link into the relevant skill. Selected intent is navy. Inline SVG symbols use consistent rounded strokes.

### Motion and Feedback

Actual implementation timings take precedence over the earlier direction brief: view entry is 280ms with 14px horizontal travel; lesson panes are 220ms with 6px vertical travel; starter content is 240ms with 10px vertical travel. The shared easing is `cubic-bezier(.16,1,.3,1)`. Hover and state transitions run 150–200ms. Copy feedback updates the button and shows a toast for 3500ms.

The explicit Motion on/off control removes CSS animation and transition and prevents the starter’s Web Animations effect. The operating-system reduced-motion preference also removes those effects; the control then reads “Reduced motion” and is disabled. The manual toggle is not persisted across reloads. No perpetual animation is implemented.

## Do's and Don'ts

### Do:

- Do preserve visible selected, hover, and keyboard-focus states.
- Do keep original-source credits beside adapted lessons.
- Do honor both the motion toggle and the operating-system reduced-motion preference.
- Do use the system UI stack consistently for operational controls and reading.

### Don't:

- Don’t add shadows to the current flat surface system without a deliberate design change.
- Don’t use animation to delay access to a control or instruction.
- Don’t present Toolkit adaptations as upstream authorship.

### Interactive motion
The home starter uses a floating intent icon, rotating orbit lines, and sequential step cues. Changing the starting choice swaps idea, code, and debugging illustrations. Navigation icons respond to hover and keyboard focus; primary arrows shift toward the destination and copied prompts draw a checkmark. Loops pause when the starter leaves the viewport or the document is hidden. Motion off and OS reduced motion disable animations.

### Spark X identity
The approved Spark X direction is implemented as a scalable SVG: deep teal X, detached upper-right arm, coral four-point spark, and mint rounded-square background. The header and favicon use the SVG; install icons are rendered from that same source.
