---
title: AI Playground
publishDate: 2025-10-19
img: /assets/ai-playground-screenshot.png
img_alt: Soft pink and baby blue water ripples together in a subtle texture.
description: |
  A Full-Stack, Cloud-Native Showcase of AI Integration and Decoupled Architecture
tags:
  - Full-Stack
  - FastAPI
  - Next.js
  - Google Cloud
---

<div class="flex flex-wrap gap-4 mb-8">
  <a href="https://aiplayground.keifer.dev" target="_blank" rel="noopener noreferrer" class="bg-primary text-primary-foreground hover:bg-primary/90 px-4 py-2 rounded-md font-semibold inline-block">
    View Live Project
  </a>
  <a href="https://github.com/keifererikson/ai-playground" target="_blank" rel="noopener noreferrer" class="bg-secondary text-secondary-foreground hover:bg-secondary/90 px-4 py-2 rounded-md font-semibold flex gap-1">
    <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" {...props}>
      <path fill="currentColor" d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5c.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34c-.46-1.16-1.11-1.47-1.11-1.47c-.91-.62.07-.6.07-.6c1 .07 1.53 1.03 1.53 1.03c.87 1.52 2.34 1.07 2.91.83c.09-.65.35-1.09.63-1.34c-2.22-.25-4.55-1.11-4.55-4.92c0-1.11.38-2 1.03-2.71c-.1-.25-.45-1.29.1-2.64c0 0 .84-.27 2.75 1.02c.79-.22 1.65-.33 2.5-.33s1.71.11 2.5.33c1.91-1.29 2.75-1.02 2.75-1.02c.55 1.35.2 2.39.1 2.64c.65.71 1.03 1.6 1.03 2.71c0 3.82-2.34 4.66-4.57 4.91c.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2" />
    </svg>
    <p>
    View Source Code
    </p>
  </a>
</div>

This project is a "clean-room" implementation of the core architecture from a proprietary, NDA-protected commercial project I led. I built the AI Model Playground from first principles to demonstrate my end-to-end capabilities in designing, building, and deploying a modern, cloud-native application.

It is an interactive web application that allows users to select, configure, and test text generation and embedding models from multiple providers, such as Gemini and Anthropic.

### The Decoupled Architecture

- **Backend:** A containerized **FastAPI (Python)** application deployed on **Google Cloud Run**. It serves a REST API and manages all AI provider logic and abstraction.
- **Frontend:** A modern **Next.js (React)** and **Shadcn/UI** application deployed on **Vercel**. It consumes the backend API and manages all client-side state using **React Context**.
- **Database:** A serverless **PostgreSQL** database persists all application settings, such as the current model and temperature.

### Key Features & Technical Highlights

- **Dynamic Provider Management:** The backend uses an abstract `LLMProvider` base class, allowing new AI providers to be added in a "plug-and-play" manner.
- **Stateful Configuration:** User-defined settings are saved to the Postgres database and globally managed on the frontend with a React Context.
- **Live AI Testing:** Users can send test prompts directly to the configured model and receive real-time responses from the selected provider.
- **Embedding Generation:** For supported providers like Gemini, users can generate and view vector embeddings for any given text input.
- **Secure Endpoint Access:** API routes that interact with paid AI services are protected, requiring a valid Access Code to prevent unauthorized use.
