<div align="center">

  # Daylight

  **A calm, calendar-based daily planner that keeps all task data in your browser.**

  ![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=000)
  ![HTML5](https://img.shields.io/badge/HTML5-Semantic-E34F26?logo=html5&logoColor=white)
  ![CSS3](https://img.shields.io/badge/CSS3-Responsive-1572B6?logo=css3&logoColor=white)
</div>

## Overview

Daylight is a lightweight daily-planning web app for organizing tasks by date and time. It uses only HTML, CSS, and JavaScript and stores tasks locally, so it works without an account or backend.

## Features

- Month calendar with previous/next navigation.
- Visible indicators for dates that contain tasks.
- Add, edit, complete, and delete tasks.
- Time-ordered daily timeline.
- Optional notes for each task.
- Four visual task types: Focus, Light, Deep Work, and Personal.
- “Next moment” card highlighting the next incomplete task.
- Daily completion summary and progress ring.
- Jump-to-today navigation.
- Responsive desktop and mobile layouts.
- Light and dark interface modes.
- Task persistence through `localStorage`.
- Basic output escaping before user-entered text is rendered.

## Run locally

No dependency installation or build process is required.

```bash
git clone https://github.com/Mateeoow/Todo.git
cd Todo
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). Opening `index.html` directly also works in most browsers.

## Project structure

```text
index.html   Semantic planner layout and task dialog
style.css    Visual system, timeline, calendar, themes, and responsive rules
app.js       Task CRUD, calendar state, rendering, progress, and persistence
```

## Data and privacy

Tasks are saved under the `daylight-tasks` key in the current browser's `localStorage`. No task data is sent to a server. Clearing site data or switching browsers/devices will remove or separate the task list.

## Current limitations

- No account or cross-device synchronization
- No reminders or push notifications
- No recurring-task rules
- Theme choice is session-based rather than saved permanently

## Possible next steps

- Persist the selected theme
- Add task search and filters
- Add recurring tasks and reminders
- Support export/import and optional cloud sync

## Author

Built by [Martin Gayem](https://github.com/Mateeoow) as a vanilla JavaScript productivity project.
