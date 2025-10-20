---
title: The Agile Dad (In Progress)
publishDate: 2025-10-20
img: /assets/the-agile-dad.png
img_alt: A Kanban board showing the agile development process for the fitness tracker.
description: |
  A full-stack, cloud-native Progressive Web App (PWA) designed for simple, effective workout and body-weight logging.
tags:
  - Full-Stack
  - .NET
  - Next.js
  - PostgreSQL
  - PWA
---

<div class="flex flex-wrap gap-4 mb-8">
  <a class="bg-secondary/50 text-secondary-foreground/70 px-4 py-2 rounded-md font-semibold inline-block cursor-not-allowed" title="Coming Soon!">
    View Live Project (Coming Soon)
  </a>
  <a href="https://github.com/keifererikson/the-agile-dad" target="_blank" rel="noopener noreferrer" class="bg-secondary text-secondary-foreground hover:bg-secondary/90 px-4 py-2 rounded-md font-semibold flex gap-1">
    <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24">
      <path fill="currentColor" d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5c.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34c-.46-1.16-1.11-1.47-1.11-1.47c-.91-.62.07-.6.07-.6c1 .07 1.53 1.03 1.53 1.03c.87 1.52 2.34 1.07 2.91.83c.09-.65.35-1.09.63-1.34c-2.22-.25-4.55-1.11-4.55-4.92c0-1.11.38-2 1.03-2.71c-.1-.25-.45-1.29.1-2.64c0 0 .84-.27 2.75 1.02c.79-.22 1.65-.33 2.5-.33s1.71.11 2.5.33c1.91-1.29 2.75-1.02 2.75-1.02c.55 1.35.2 2.39.1 2.64c.65.71 1.03 1.6 1.03 2.71c0 3.82-2.34 4.66-4.57 4.91c.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2" />
    </svg>
    <p>
      View Source Code
    </p>
  </a>
</div>

This project is my personal fitness logger, built from scratch to solve my own needs. I'm building it as a Progressive Web App (PWA) to be fast, reliable, and installable on any device.

It's currently in active development. I'm using this page to document the process and showcase my approach to product definition, system architecture, and agile execution.

### The Architecture

The system is designed as a decoupled, full-stack application:

- **Frontend:** A **React PWA** (built with Next.js) that can be installed on a mobile device.
- **Backend API:** A **.NET** application serving a REST API to manage users and workout data.
- **Database:** A **PostgreSQL** database to persist all user and workout information.

### The Plan (MVP)

The Minimum Viable Product (MVP) is defined by a small, focused set of user stories that deliver the core value:

- **US-01:** As a new user, I want to create an account with my email and a password.
- **US-02:** As a user, I want to be able to log my cardio workouts.
- **US-03:** As a user, I want to be able to log my weight machine workouts.
- **US-04:** As a user, I want to be able to log my body weight.

### Current Status

Development is being tracked on an agile GitHub Project Kanban board. As of October 2025, the initial backend and frontend structures are the priority.
