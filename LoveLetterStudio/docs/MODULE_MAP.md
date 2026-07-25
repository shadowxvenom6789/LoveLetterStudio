# Love Letter Studio Module Map

This document defines where every feature belongs.

Always add code to the correct module.

Avoid placing unrelated code into existing files.

---

# Backend

File

app.py

Owns

- Local server
- Configuration loading
- Letter loading
- Static file serving
- Export backend
- Future API endpoints

Do NOT place

- HTML
- CSS
- Animations
- UI logic

---

# HTML

File

templates/index.html

Owns

- Page structure
- Semantic HTML
- Containers
- Components
- Accessibility

Do NOT place

- CSS
- JavaScript logic
- Python code

---

# CSS

File

static/css/style.css

Owns

- Colors
- Layout
- Typography
- Animations
- Responsive design
- Themes
- Visual effects

Do NOT place

- JavaScript
- HTML
- Python

---

# JavaScript

File

static/js/script.js

Owns

- Animations
- Event listeners
- User interaction
- Effects
- Media controls
- Dynamic updates

Do NOT place

- CSS
- HTML
- Backend logic

---

# Letters

Folder

letters/

Owns

- TXT letters
- Markdown letters
- Future templates

---

# Images

Folder

assets/images/

Owns

- Embedded images
- Gallery images
- Decorative assets

---

# Audio

Folder

assets/audio/

Owns

- Background music
- Voice messages
- Sound effects

---

# Videos

Folder

assets/videos/

Owns

- Embedded videos
- Memory videos

---

# Fonts

Folder

assets/fonts/

Owns

- Local fonts
- Signature fonts
- Theme fonts

---

# Themes

Folder

assets/themes/

Owns

- Theme configuration
- Theme assets
- Theme colors

---

# Exports

Folder

exports/

Owns

- HTML exports
- PDF exports
- Image exports

---

# Documentation

Folder

docs/

Owns

- Project documentation
- AI instructions
- Development roadmap

---

# Future Modules

Theme Manager

Responsible for

- Theme loading
- Theme switching
- Theme settings

---

Media Manager

Responsible for

- Images
- Videos
- Audio
- Voice notes

---

Animation Manager

Responsible for

- Envelope animation
- Paper unfolding
- Typewriter
- Particles
- Effects

---

Editor Manager

Responsible for

- Editing
- Preview
- Auto save
- File management

---

Export Manager

Responsible for

- HTML export
- PDF export
- PNG export
- Printing

---

Settings Manager

Responsible for

- User preferences
- Theme selection
- Animation settings

---

Communication Rules

Backend communicates with Frontend.

Frontend communicates with CSS and JavaScript.

JavaScript may modify HTML.

CSS never contains logic.

Python never controls animations directly.

---

AI Rules

Before implementing a feature

1. Identify the correct module.

2. Modify only that module.

3. If a new module is needed, create it.

4. Never duplicate existing functionality.

5. Keep modules independent.

6. Update this file if a new module is introduced.
