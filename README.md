# ⚡ QuizPrep

A clean, modern, and privacy-first web application for practicing quizzes and simulating exams. Turn study notes, documentation, or textbooks into interactive tests in seconds.

> **Note:** This entire application is **vibecoded** — sculpted end-to-end through iterative prompts and conversational coding with AI. Zero boilerplate bloat, pure functional vibes.

---

## ✨ Features

- **Dual Testing Modes**:
  - **Quiz Mode**: Learn as you go with instant feedback. Choose between instant-check upon selecting an option or explicit submission.
  - **Exam Mode**: Simulates real test conditions. Answers and feedback are hidden until the final submission.
- **Multiple Question Formats**:
  - **Multiple Choice (MC)**: Supports pipe-separated choices.
  - **Write-in (WI)**: Evaluated using **Regular Expressions (Regex)** with support for both case-sensitive and case-insensitive matching.
- **Smart Randomization**:
  - Shuffle question order independently.
  - Shuffle multiple-choice options on each attempt so you never memorize answer positions.
- **Modern Adaptive Theme**:
  - Sleek segmented pill-slider to toggle between **Light**, **Dark**, and **System Auto**.
  - Dynamically responds to OS dark/light mode changes in real time.
- **Flagging & Review**:
  - Flag tricky questions during tests for later review.
  - Sort and filter results at the end by *All*, *Wrong Only*, or *Flagged Only*.
- **LLM-Friendly (AI Workflow)**:
  - Built-in one-click prompt template for ChatGPT, Claude, or Gemini.
  - Generate quiz-ready CSV data from your notes and paste it directly into the app (no need to save/download files).
- **100% Client-Side & Private**:
  - Runs entirely in your browser using `localStorage`. No backend, no trackers, no external databases.

---

## 🚀 Quick Start (GitHub Pages)

### 1. Fork or Create Repository
1. Create a new repository on GitHub (e.g., `quiz-app`) and ensure it is set to **Public**.
2. Add the `index.html` file to the root of your repository.

### 2. Enable GitHub Pages
1. Go to your repository's **Settings** tab.
2. Select **Pages** from the left sidebar.
3. Under **Branch**, select `main` (or `master`) and `/ (root)`.
4. Click **Save**.
5. Wait 1–2 minutes, and your site will be live at:
