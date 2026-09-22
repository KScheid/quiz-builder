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
5. Wait 1–2 minutes, and your site will be live at: https://github.com/KScheid/quiz-builder/blob/main/README.md

---

## 🤖 The LLM Workflow

You don't need to manually write questions. Use any AI assistant to build tests from your materials:

1. Open **QuizPrep** and click **"📋 Copy Prompt"** in Step 1.
2. Paste the prompt into ChatGPT, Claude, or Gemini, followed by your lecture notes, textbook excerpt, or study guide.
3. Copy the raw CSV code block the AI generates.
4. Paste the text directly into the **"Option 1: Paste CSV Data"** field in QuizPrep.
5. Click **Start Session**!

---

## 📄 CSV Format Specification

If you prefer to create or store your quizzes as `.csv` files, use this structure:

```csv
Question,Type,Options,Answer,CaseSensitive
What is the capital of France?,MC,London|Paris|Berlin|Madrid,Paris,FALSE
Type the word "apple",WI,,^apple$,TRUE
Who wrote Hamlet?,MC,Charles Dickens|William Shakespeare|Mark Twain,William Shakespeare,FALSE
What is 2 + 2?,WI,,^4$,FALSE
Does this regex match a 3 digit number (e.g. 123)?,WI,,^\d{3}$,FALSE

Column Reference
Column	Allowed Values	Description
Question	String	The prompt or question text.
Type	MC or WI	Multiple Choice (MC) or Write-in (WI).
Options	Pipe-delimited (|)	The list of choices for MC. Leave blank for WI.
Answer	String / Regex	For MC, must match an option verbatim. For WI, provide a Regex pattern (e.g., ^answer$).
CaseSensitive	TRUE or FALSE	Controls whether write-in regex matching is case-sensitive (ignored for MC).
🛠️ Tech Stack
HTML5 & Vanilla JavaScript (Zero frameworks, zero build steps)
CSS Custom Properties (Smooth dark/light transitions and glassmorphism)
PapaParse (Fast, in-browser CSV parsing)
GitHub Pages (Free static hosting)
🔒 Privacy
QuizPrep does not send your notes, questions, or quiz results to any server. Everything is parsed in your browser and saved to your device's localStorage.
💡 About
Created with focus, flow, and caffeine. Vibecoded from scratch. Feel free to fork, tweak, and expand!
