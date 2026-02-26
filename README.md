AccessLearn AI
​The Inclusive, AI-Powered Learning Management System
​AccessLearn AI is a specialized learning management system designed with a deep accessibility philosophy. It provides an inclusive environment specifically for users with visual and hearing impairments, using a lightweight Vanilla JS architecture and AI-driven study tools.
​Key Features
​Advanced Accessibility System
​Managed via a centralized global state, the platform adapts instantly to user needs:
​Deaf Mode: Forces subtitle overlays on all video content, replaces audio cues with visual alerts, and enhances interactive states with high-visibility borders.
​Blind / High Contrast Mode: Switches to a specialized Yellow-on-Black theme for maximum readability. A custom AccessibilityEngine using the Web Speech API narrates page content and navigation changes.
​ARIA-First Design: Strict enforcement of ARIA roles across all components for seamless screen reader compatibility.
​AI-Integrated Learning
​AI Doubt Solver: A built-in chat panel that acts as a tutor by scanning transcripts to answer contextual questions in real-time.
​Automated Notes: Generates structured, AI-summarized notes based on video content for efficient revision.
​Interactive Transcripts: Searchable, timestamped sidebars that highlight as the video progresses.
​Smart Content Delivery
​Hybrid Video Player: Automatically detects and renders both direct MP4 files and YouTube embeds.
​Auto-Seeding: Ensures the Firestore database is populated by generating boilerplate courses on the first launch.
​Technology Stack
​Frontend: Vanilla JavaScript (ES6+), HTML5
​Styling: Tailwind CSS
​Icons: Lucide Icons
​Backend: Firebase Authentication
​Database: Cloud Firestore (NoSQL)
​Routing: Custom Vanilla JS Hash Router
​Project Architecture
​The project follows a modular SPA architecture to maintain performance for assistive tools.
​index.html: Main shell and Tailwind configuration.
​js/store.js: Global state management for Auth and Accessibility modes.
​js/accessibility-engine.js: Logic for Web Speech API and Text-to-Speech.
​js/pages/video.js: Video UI and AI Assistant integration.
​Database Schema (Firestore: courses)
​title (String): Name of the course
​category (String): e.g., Frontend, Design
​level (String): Beginner, Intermediate, or Advanced
​video_url (String): Firebase Storage or YouTube Link
​duration (String): e.g., 4h 30m
​Setup and Installation
​Clone the Repository:
git clone https://github.com/your-username/accesslearn-ai.git
​Firebase Configuration:
Create a project in the Firebase Console, enable Authentication and Firestore, and add your config to js/firebase-config.js.
​Launch:
Open index.html via a local server like VS Code Live Server.
