<h1 align="center">📝 Notes App</h1>
<p align="center">A productivity-focused Android notes app built with MVVM and Room</p>

<p align="center">
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/MVVM-4285F4?style=flat" />
  <img src="https://img.shields.io/badge/Room-3DDC84?style=flat" />
</p>

---

## Overview

Notes App is a clean, offline-first note-taking application for Android. It focuses on a fast, distraction-free experience for capturing, organizing, and prioritizing personal notes — all persisted locally with Room.

## Features

- ✍️ Create, edit, and delete notes
- 🔍 Search across all saved notes
- ⭐ Priority-based sorting to surface what matters most
- 💾 Fully offline — all data persisted locally via Room
- 🧱 Clean, testable MVVM architecture

## Architecture

```
UI (Activity/Fragment)
      ↓
ViewModel  →  Repository  →  Room (DAO / Database)
      ↓
LiveData / StateFlow
```

- **Room** serves as the single source of truth for all note data
- **Repository layer** decouples the UI from direct database access, keeping the codebase testable
- **ViewModel** exposes observable state, keeping the UI reactive and lifecycle-aware

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Kotlin |
| Architecture | MVVM |
| Local Storage | Room |
| UI | Android Views / Jetpack Compose |

## Getting Started

### Prerequisites
- Android Studio (latest stable)

### Setup
```bash
git clone https://github.com/piyushyadav00/notes-app.git
cd notes-app
```

Open the project in Android Studio and run on an emulator or physical device — no API keys or external setup required.

## Screenshots

*(Add screenshots here — list view, create/edit screen, and search-in-action are the most useful for reviewers)*

## What This Project Demonstrates

- Designing a fully offline, local-first Android app
- Clean CRUD architecture using Room and the Repository pattern
- Practical application of MVVM for a real, everyday-use case
- Thoughtful UX details like priority-based sorting and in-app search

---

<p align="center"><i>Built by <a href="https://github.com/piyushyadav00">Piyush Yadav</a></i></p>
