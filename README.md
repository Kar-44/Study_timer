# Study Tracker & Pomodoro Timer

A lightweight, browser-based web application designed to optimize your learning process and track long-term progress. By combining the scientifically proven Pomodoro technique with comprehensive goal management, this tool helps maintain focus, prevent burnout, and visually map your journey toward major academic or professional milestones.

This was built because I feel like it is much easier to learn start something and stay motivated if we see progress. Seeing the % of estimated time goal increase is some progress and it can keep us going. I hope you will find it useful.

## Purpose & Philosophy
Effective learning requires both intense, focused study sessions and a clear overview of long-term progress. This application solves two common productivity problems:
1. **Maintaining Focus:** It uses timed intervals (Pomodoros) to break work into manageable chunks, encouraging sustained concentration while ensuring adequate rest.
2. **Tracking Progress:** It bridges the gap between daily effort and macroscopic goals. Every minute spent studying dynamically updates a visual progress ring, transforming abstract study hours into a tangible sense of achievement.

## Key Features
* **Multi-Goal Management:** Create, switch between, and manage multiple distinct study goals (e.g., "Physics Exam", "Programming Course") via a top-bar dropdown without losing your data.
* **Integrated Pomodoro Timer:** Automates the classic workflow: 25 minutes of study, 5 minutes of short break, and a 30-minute long break after every 4 completed study sessions.
* **Dynamic Progress Tracking:** Input your estimated required study hours. As the Pomodoro timer ticks during "Study Time", your logged hours automatically fill a circular progress bar. 
* **Rich Text Notes & Task Lists:** A built-in rich text editor (powered by Quill.js) allows you to jot down conclusions, structure study plans, or check off to-do lists directly beneath your goal.
* **Persistent Local Storage:** All goals, timer states, and notes are saved instantly to your browser's `localStorage`. You can close the tab or refresh the page without losing a single second of progress.

## How It Works
1. **Set a Goal:** Click **+ New Goal**, name your event, set the target date (formatted as dd/mm/yyyy), and estimate the total hours required to master the subject.
2. **Start the Timer:** Click **Start** on the Pomodoro panel. The application will track the elapsed time. Only active "Study Time" is added to your total logged hours.
3. **Follow the Cycles:** The timer tracks your active sessions. It will alert you when a phase is complete and automatically queue up the appropriate break (Short or Long) based on your session count. You can also manually skip phases.
4. **Track & Adapt:** Watch your progress circle fill up as you log hours. Use the notes section to refine your strategy, format key takeaways with bold/italics, or list specific topics for your next session using checkboxes.

## Installation & Usage
This is a standalone, client-side application requiring no server or backend installation.

1. Create a new text file on your computer and name it `index.html`.
2. Copy the entire HTML/CSS/JS code into this file and save it.
3. Double-click the `index.html` file to open it in any modern web browser (Chrome, Edge, Safari, Firefox).
4. Start tracking your study sessions immediately.

## Technologies Used
* **HTML5 & CSS3:** For a responsive, dark-mode-optimized user interface.
* **Vanilla JavaScript (ES6+):** Handles multi-state timer logic, dynamic DOM manipulation, SVG progress calculations, and state management.
* **Quill.js (via CDN):** Provides the lightweight, robust rich-text editor for notes and interactive checklists.
* **Browser LocalStorage API:** Ensures 100% local, private data persistence across browser sessions.
