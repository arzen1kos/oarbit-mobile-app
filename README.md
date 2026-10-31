<div align="center">
   <img width="100" height="100" alt="oarbit-app-logo" src="https://github.com/user-attachments/assets/b0a3eefe-9ca3-402d-9721-a73547030ff4" />
  
# OarBit | Habit & Routine Companion App 
![JavaScript](https://img.shields.io/badge/JavaScript-f6de07?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-f68507?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/css-c159f9?style=for-the-badge&logo=css&logoColor=white)

~✦~

`OarBit` is a mobile routine management app designed to help users build healthy habits through scheduled reminders and optional focus-enforcement periods. Unlike traditional reminder apps, `OarBit` can temporarily restrict app usage after a reminder is triggered, encouraging users to complete activities such as stretching, walking, exercising, hydration, language practice, or mindfulness exercises. Developed as part of the **BCDE213 Interactive Media Development** course portfolio, the project explores user-centred design, mobile interaction patterns, and behaviour-driven habit formation.

</div>

## Branch notes: `dev`

**Overview:** Development branch for upcoming features beyond v1.0.0.

**Notes**

The current main release provides task management, timer functionality, and statistics tracking in vanilla JavaScript. Future iterations will explore enhanced reminder scheduling, notification systems, habit-building workflows, optional focus-enforcement mechanics, UI/UX refinements, and architectural improvements as the project evolves.

**Status**: v1.0.0 - Initial Portfolio Release

## Features

- Create custom routines and reminders
- Configure fixed or recurring reminder intervals
- Set reminders for specific times of day
- Optional focus-lock periods after reminders trigger
- Support for short tasks (drink water, vocabulary prompt)
- Support for longer activities (stretching, exercise, walking)
- User-friendly routine management interface
- Customisable reminder schedules and durations

## Architecture at a Glance

```mermaid
flowchart LR
    U[User] --> A[Mobile App]

    A --> R[Routine Manager]
    A --> N[Notification Service]
    A --> L[Lock Controller]

    R --> D["(Local Storage)"]

    N --> T[Reminder Trigger]

    T --> L
    T --> U

    L --> F[Focus Lock Period]
```

## User Journey

```mermaid
journey
    title Task Creation and Completion
    section Create Routine
      Open App: 5: User
      Create Task: 5: User
      Configure Schedule: 4: User
      Set Lock Duration: 4: User

    section Reminder Trigger
      Receive Notification: 5: User
      Open Task Prompt: 4: User

    section Accountability
      Complete Activity: 5: User
      Lock Expires: 4: System
      Return to Work: 5: User
```

## Quick Setup

```bash
# Clone repository
git clone https://github.com/arzen1kos/oarbit-mobile-app.git
cd oarbit-mobile-app

# Install dependencies
npm install

# Start development server
npm run dev
```

## Academic Integrity Notice
>
> This repository was developed solely as a personal academic portfolio project for BCDE213 Interactive Media. All submitted coursework, assessments, design artefacts, and implementation work were completed in accordance with the academic integrity policies and assessment requirements of Ara Institute of Canterbury. This project is provided for portfolio and educational purposes only and should not be submitted, copied, or represented as another student's original work.

---

Created by Arsenie — 2024
