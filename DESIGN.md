---
name: "序列 · Sequence"
description: "A restrained desktop workspace for traceable data-processing tasks."
colors: {"bg": "#f7f8fa", "surface": "#fff", "sidebar": "#f1f3f7", "ink": "#283247", "muted": "#667188", "subtle": "#788298", "border": "#e5e8ee", "strong": "#cbd1dd", "primary": "#303d5c", "primary-hover": "#23304e", "blue": "#42659d", "blue-bg": "#edf3fb", "green": "#347663", "green-bg": "#edf6f1", "red": "#b64646", "red-bg": "#fcf0f0", "amber": "#8d682d", "amber-bg": "#faf4e7", "ring": "#5d78a7"}
typography: {"headline": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "27px", "fontWeight": 650, "lineHeight": 1.3, "letterSpacing": "-0.02em"}, "dialog-title": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "20px", "fontWeight": 600, "lineHeight": 1.5, "letterSpacing": "-0.02em"}, "title": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "15px", "fontWeight": 600, "lineHeight": 1.5}, "body": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "14px", "fontWeight": 400, "lineHeight": 1.5}, "task-name": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "14px", "fontWeight": 500, "lineHeight": 1.5}, "label": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "12px", "fontWeight": 500, "lineHeight": 1.5}, "metadata": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "12px", "fontWeight": 400, "lineHeight": 1.5}, "log": {"fontFamily": "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"PingFang SC\", \"Microsoft YaHei\", sans-serif", "fontSize": "13px", "fontWeight": 400, "lineHeight": 1.7}}
rounded: {"status": "4px", "control": "6px", "surface": "8px", "panel": "9px", "dialog": "12px"}
spacing: {"space-1": "4px", "space-2": "8px", "space-3": "12px", "space-4": "16px", "space-6": "24px", "space-8": "32px"}
components: {"button-primary": {"backgroundColor": "{colors.primary}", "textColor": "{colors.surface}", "rounded": "{rounded.control}", "padding": "8px 15px", "typography": "{typography.label}"}, "button-primary-hover": {"backgroundColor": "{colors.primary-hover}"}, "button-secondary": {"backgroundColor": "{colors.surface}", "textColor": "{colors.ink}", "rounded": "{rounded.control}", "padding": "7px 13px", "typography": "{typography.label}"}, "button-ghost": {"backgroundColor": "transparent", "textColor": "{colors.muted}", "rounded": "{rounded.control}", "padding": "7px 13px"}, "input": {"backgroundColor": "{colors.surface}", "textColor": "{colors.ink}", "rounded": "{rounded.control}", "height": "39px", "padding": "9px 11px"}, "status-running": {"backgroundColor": "{colors.blue-bg}", "textColor": "{colors.blue}", "rounded": "{rounded.status}", "padding": "3px 7px", "typography": "{typography.label}"}, "panel": {"backgroundColor": "{colors.surface}", "rounded": "{rounded.panel}"}, "nav-active": {"backgroundColor": "#dfe6f1", "textColor": "#293e62", "rounded": "{rounded.control}", "height": "43px", "padding": "0 13px"}}
---
# Design System: 序列 · Sequence

## Overview

**Creative North Star: "Orderly Execution"**

A cool slate shell and white work surfaces make task names, execution states, and recovery actions easy to scan. The interface is professional and restrained, with enough density for repeated desktop operations.

The technical-standard reference lands as orderly type, quiet rules, and a readable three-stage execution flow. It does not turn the application into a document or decorate the work with illustrations.

**Key Characteristics:**
- Cool neutral shell with white operational surfaces.
- Compact tables and nearby recovery actions.
- Semantic status colors paired with written labels.
- Functional SVG icons; text leads headings and content labels.

## Colors

The primary slate is quiet and decisive; semantic colors explain task state rather than decorate the shell. Values in the frontmatter are normative and extracted from the shipped stylesheet.

### Primary
- **Working Slate** (`primary`, `primary-hover`): primary creation, execution and download actions, with a darker hover state.

### Secondary
- **Processing Blue** (`blue`, `blue-bg`): running tasks and their progress.
- **Completed Green** (`green`, `green-bg`): successful work and connection indicators.
- **Failure Red** (`red`, `red-bg`): failures, invalid input and retry emphasis.
- **Queued Amber** (`amber`, `amber-bg`): waiting tasks.

### Neutral
- **Cool Canvas** (`bg`), **White Surface** (`surface`), and **Slate Shell** (`sidebar`): application, work panels and navigation.
- **Task Ink** (`ink`), **Supporting Slate** (`muted`, `subtle`): primary and supporting information.
- **Quiet Rule** (`border`) and **Control Stroke** (`strong`): separation and field/button edges.
- **Focus Blue** (`ring`): keyboard focus and search focus-within.

**The Semantic Color Rule.** Use status colors to explain execution state; keep ordinary surfaces neutral.

## Typography

The system uses the platform sans-serif stack in frontmatter, including Chinese fallbacks. There is no separate display or monospace face. Numeric IDs, counts, percentages and times use tabular numerals where assigned.

The hierarchy is a compact page headline, medium dialog heading, small section title, readable task text, and quieter metadata. The implemented page headline is 27px rather than the provisional 28px. The small uppercase English page companion remains an incidental shipped kicker; it is not canonized as a reusable heading pattern. Task names have medium weight; supporting copy remains regular. Small shell captions and auxiliary controls use the observed 10–11px range; the tiny English brand subtitle and workspace tag are incidental existing identity details, not a general label style.

**The Readable Task Data Rule.** Keep task data at 14px, IDs, timestamps, and status at 12px, and execution-log messages at 13px.

## Layout

This is a desktop-only application: body minimum width is 1040px. The fixed sidebar is 216px wide, the topbar is 66px high, and the main content uses 34px horizontal padding with a 1600px maximum width. Repeated spacing follows the frontmatter rhythm. The overview is one horizontal strip and the work panel combines filter tabs, toolbar, table and pagination.

At viewport widths up to 1200px, the sidebar becomes 190px, content padding becomes 24px, the overview sync label is hidden, and the table retains an 810px minimum width inside a horizontal scroll container. At widths from 1600px, top spacing increases and table rows become 76px rather than the usual 70px. These are desktop density adjustments, not a mobile design.

## Elevation & Depth

White surfaces, cool backgrounds and thin neutral rules establish depth at rest. Ordinary panels have no shadow. The toast uses `0 6px 22px #18263a26`; dialogs use `0 16px 64px #1720332b`, with a `#1c26394d` backdrop. There are no gradients.

**The Flat Work Surface Rule.** Reserve cast shadows for dialogs and toast feedback; ordinary panels stay flat.

## Shapes

Controls have gently rounded corners, small status badges are compact rectangles, and panels have slightly softer corners. Centered dialogs use the largest radius; the full-height right-hand task detail uses square corners. Circles are reserved for avatars, small state dots and execution-stage markers. The neutral hairline and dots in the log timeline convey sequence, not a colored card accent border.

## Components

### Buttons

Primary actions use dark slate with white text. Secondary buttons use white with the stronger neutral border; ghost actions remove the border and use muted text. Primary minimum height is 37px; regular controls are 34px. Hover changes color and border over 150ms ease. Disabled buttons have 45% opacity and a not-allowed cursor. Destructive actions use red text and a pale red border. Text actions and square icon buttons support compact rows.

### Inputs / Fields

Form inputs and selects have 39px height, neutral stroke and white fill. Search and filter controls are 34px high. Search uses a containing focus border; global keyboard focus uses a 2px ring with 3px offset. Invalid task-name input turns its border red and links to an alert message. Submission disables fields and duplicate actions while preserving entered values.

### Navigation

The sidebar uses compact horizontal links, functional line icons, a muted default state and a tonal active fill with semibold text. Filter tabs use a bottom underline and count pills; their implemented semantics are pressed buttons in a labeled group, not ARIA tabs. Navigation is desktop-only.

### Chips

Statuses are written labels with a tiny same-color dot: queued, running, succeeded, failed and cancelled. Their semantic backgrounds are pale; cancelled uses the neutral default. Running rows add a numeric percentage and a thin progress track. Color never carries the state alone.

### Cards / Containers

The overview and table panel use white fill, thin neutral border and no shadow. The overview has 22px by 24px internal padding; toolbar padding is 17px by 20px. Table rows have hover and selected tonal fills. Loading uses static pale skeleton bars; empty and request-error states provide relevant recovery actions.

### Execution Details and Dialogs

Task detail is a 556px full-height right-side native modal dialog (maximum 90vw), with its own scrolling body and stationary footer. Its three-stage sequence is read, process, export; written labels, numbered markers and functional completion/error icons explain progress. Failed tasks expose the reason and retry; succeeded tasks expose summary, preview and CSV download; active tasks offer cancellation.

Creation is a centered 540px native dialog. Dataset preview is 660px and about is 500px. Native modal behavior supplies focus containment and Escape dismissal; creation blocks Escape during submission. The task-list `/` shortcut focuses search only outside editable fields and when no dialog is open. Focus remains visible; icon-only controls carry accessible labels.

Progress widths transition over 400–500ms ease; refresh/submission icons spin over 1.2s linear. The reduced-motion media query disables animations and transitions. Toasts use status semantics and a labeled close control.

## Do's and Don'ts

### Do:
- **Do** pair status color with its written label.
- **Do** keep recovery and download actions close to the relevant task.
- **Do** use functional inline SVG icons with accessible text or button labels.
- **Do** preserve the desktop density and visible keyboard focus.

### Don't:
- **Don't** add arbitrary lightning or decorative icons; headings, overview labels, and content labels default to text.
- **Don't** use colored left-side accent borders on cards or notices.
- **Don't** add gradients or oversized metric cards that displace the working table.
- **Don't** imply that a mobile layout exists.
