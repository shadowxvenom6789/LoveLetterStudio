# Love Letter Studio Architecture

## Project Architecture

Love Letter Studio follows a modular architecture.

Each component has one responsibility.

Components communicate with each other instead of containing duplicated logic.

---

# High Level Overview

Python Backend
        │
        ▼
Loads Letter Data
        │
        ▼
Serves HTML Page
        │
        ▼
Browser
        │
        ▼
HTML Layout
        │
        ▼
CSS Styling
        │
        ▼
JavaScript Logic
        │
        ▼
Animations + User Interaction

---

# Backend

File

app.py

Responsibilities

• Start local server

• Load configuration

• Load letter files

• Serve HTML

• Serve static assets

• Handle future export features

Backend should remain lightweight.

Business logic should stay minimal.

---

# Frontend

## HTML

Responsible for

• Layout

• Structure

• Accessibility

No animation logic.

No styling logic.

---

## CSS

Responsible for

• Colors

• Themes

• Layout

• Responsive design

• Animations

No application logic.

---

## JavaScript

Responsible for

• User interaction

• Envelope animation

• Letter opening

• Effects

• Media controls

• Dynamic updates

No styling.

---

# Assets

Images

assets/images/

Audio

assets/audio/

Videos

assets/videos/

Fonts

assets/fonts/

Themes

assets/themes/

Exports

exports/

Letters

letters/

---

# Documentation

PROJECT.md

Project vision

RULES.md

Development rules

STYLEGUIDE.md

Visual rules

TASKS.md

Development roadmap

CURRENT_STATE.md

Current development progress

CHANGELOG.md

Project history

PROMPTS.md

Reusable AI prompts

ARCHITECTURE.md

System architecture

FILE_STRUCTURE.md

Folder explanations

---

# Future Modules

Theme Manager

Letter Manager

Media Manager

Export Manager

Animation Manager

Settings Manager

Plugin System (optional)

---

# Data Flow

Letter

↓

Python

↓

HTML

↓

JavaScript

↓

Animation

↓

User

---

# Design Principles

One responsibility per module.

Avoid duplicated logic.

Keep modules independent.

Prefer extending modules instead of replacing them.

Minimize coupling.

Maximize readability.

---

# AI Guidelines

When implementing a feature:

1. Identify the responsible module.

2. Modify only that module.

3. Avoid unrelated changes.

4. Preserve existing architecture.

5. Update documentation if architecture changes.

Architecture stability is more important than short-term convenience.
