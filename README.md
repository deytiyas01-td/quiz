# Interactive Quiz Website

A modern, responsive, and feature-rich interactive quiz application built with **HTML5**, **Tailwind CSS**, and **Vanilla JavaScript (ES6+)**[cite: 2]. This application is designed for seamless knowledge assessment with dynamic question loading, real-time score tracking, instant visual feedback, and state-managed restarts[cite: 2].

---

## 🎯 Objective & Scope

* Add questions, score tracking, feedback, restart functionality, and responsive UI[cite: 2].
* Provide an engaging user experience with touch-friendly mobile navigation and high-contrast color-coded state indicators[cite: 2].

---

## 🛠️ Recommended Stack & Tools

* **Markup:** HTML5
* **Styling:** Tailwind CSS (via CDN)
* **Logic & State:** Vanilla JavaScript (ES6+ DOM Manipulation)
* **Data Source:** JSON dataset containing structured question banks and detailed explanations[cite: 2].

---

## 🧠 State Management Logic

The application relies on a robust client-side state management pattern using vanilla JavaScript to handle user interaction without requiring full page reloads:

1. **Global State Variables:**
   * `quizData`: Stores the array of questions fetched from the JSON dataset[cite: 2].
   * `currentQuestionIndex`: Tracks the index of the currently active question.
   * `score`: Accumulates the user's correct answers in real time[cite: 2].
   * `isAnswered`: Boolean flag that locks option buttons after a choice is made to prevent multiple submissions[cite: 2].

2. **Flow & UI Transitions:**
   * **Initialization:** Fetches the question bank from `questions.json`, sets total counts, and renders the first question[cite: 2].
   * **Answer Selection:** When an option is clicked, `isAnswered` turns `true`, options are disabled, correct/incorrect visual feedback classes are applied instantly, and the explanation box is revealed[cite: 2].
   * **Progress Tracking:** The progress bar width and question number indicator update dynamically upon every answer transition[cite: 2].
   * **State Reset (Restart):** The `restartBtn` event listener resets `currentQuestionIndex` and `score` back to zero and re-renders the initial state seamlessly without a page reload[cite: 2].

---

## ✅ Acceptance Criteria Checklist

* [x] **Accurate Scoring & Progress:** Score and progress update accurately upon every question answer[cite: 2].
* [x] **Single Submission Enforcement:** Prevents multiple submissions on the same question once answered[cite: 2].
* [x] **Responsive & Touch-Friendly:** Fully optimized layout for mobile phone screens and desktop viewports[cite: 2].
* [x] **Dynamic Feedback:** Instant visual feedback (color-coded correct/incorrect states) upon answer selection[cite: 2].
* [x] **Seamless Restart:** Quiz restart button successfully resets state without a full page reload[cite: 2].

---

## 🚀 Deliverables Included

* **Web Project Codebase:** Modular or single-file HTML/CSS/JS implementation.
* **JSON Dataset (`questions.json`):** Structured file containing question banks and explanations[cite: 2].
* **Documentation (`README.md`):** Comprehensive project documentation detailing state management and architecture[cite: 2].
