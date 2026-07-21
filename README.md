================================================================================
                                ACCESSLEARN AI
                  Project Documentation & Technical Profile
================================================================================

1. LIVE DEMO
--------------------------------------------------------------------------------
Deploy Link: https://69a07d60033ec05ed571f58b--thunderous-chebakia-3f9efa.netlify.app/


2. INTRODUCTION
--------------------------------------------------------------------------------
AccessLearn AI is a specialized, accessibility-first Learning Management System 
(LMS) engineered to provide a barrier-free, inclusive educational experience. 
Architected specifically for users with visual and hearing impairments, the 
application breaks away from bloated frameworks, utilizing a lightweight, 
hyper-performant Vanilla JavaScript Single Page Application (SPA) design. It 
pairs semantic HTML5 structures with real-time AI study enhancements to deliver 
optimized learning to every student.


3. KEY FEATURES
--------------------------------------------------------------------------------
[A] Advanced Accessibility System
Driven by a centralized global state engine, the platform instantly mutates its 
configuration to serve specific user needs without requiring page reloads:

  * Deaf Mode: 
    Automatically forces subtitle overlays across all video playbacks, strips 
    out critical audible alerts in favor of visual screen flashes/banners, and 
    implements high-visibility focus indicator rings around interactive 
    elements.

  * Blind / High Contrast Mode: 
    Instantly drops standard palettes for a high-contrast Yellow-on-Black 
    readability theme. A custom automated script tracks user focus, routing 
    text boundaries directly into the Web Speech API (speechSynthesis) to act 
    as an on-the-fly screen reader.

  * ARIA-First Design: 
    Native enforcement of ARIA attributes, semantic landmarks, roles, and 
    logical tab indexing guarantees clean accessibility compatibility with 
    traditional hardware screen readers.

[B] AI-Integrated Learning
  * AI Doubt Solver: 
    An on-screen panel hosting an artificial intelligence tutor. It processes 
    video transcripts synchronously to answer context-aware questions during 
    the lecture.

  * Automated Notes: 
    Condenses audio and transcript timelines into clean, bulleted summaries to 
    provide rapid post-lecture revision resources.

  * Interactive Transcripts: 
    A side-panel text layout mapping time markers directly to the media stream, 
    highlighting lines sequentially as the playback engine advances.

[C] Smart Content Delivery
  * Hybrid Video Player: 
    A wrapper logic layer parsing inputs to seamlessly render raw cloud-hosted 
    MP4 links or cross-origin YouTube video embeds inside a standardized user 
    interface.

  * Auto-Seeding Engine: 
    A runtime database initialization flag that intercepts execution on the 
    first launch. If Firestore returns empty collections, it programmatically 
    provisions standard course boilerplate entries.


4. TECHNOLOGY STACK
--------------------------------------------------------------------------------
  * Frontend Framework : Vanilla JavaScript (ES6+ Module Architecture)
  * Styling Engine     : Tailwind CSS
  * Iconography        : Lucide Icons
  * Authentication     : Firebase Authentication
  * Database Management: Cloud Firestore (NoSQL Document Store)
  * Routing Strategy   : Custom Client-Side Hash Router (window.location.hash)

================================================================================
