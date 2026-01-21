# FT_TRANSCENDENCE

<p align="center" width="100%">
    <img width="33%" src="https://github.com/natalie-mein/images/blob/main/ft_transcendencem.png">
</p>

## Project Overview

Ft_transcendence is a full-stack web application and multiplayer gaming platform built as part of the 42 curriculum.
The project combines real-time gameplay, user management, and tournament features  with secure authentication.
Players can compete in a classic Pong game against friends, or random opponents, and manage their profiles.

## Key Features

- Real-time Pong Gameplay – Play against another player.<br>
- User Management – Registration, login, and profile customization.<br
- Secure Authentication – JWT-based login and Two-Factor Authentication (2FA).<br>
- Tournaments – Participate in competitive tournaments.<br>
- Multi-player Support – Add a third player for some fun and chaos.<br>
- Containerized Deployment – Fully managed with Docker Compose.<br>

## Tech Stack

### Frontend

    React – Component-based UI
    TypeScript – Type-safe development
    Tailwind CSS – Utility-first styling

### Backend & Architecture

    Node.js + Fastify – High-performance backend services
    TypeScript – Type-safe development
    SQLite – Lightweight database for persistence
    Prisma – ORM for structured and maintainable database management
    WebSockets – Real-time communication
    Docker & Docker Compose – Simplified deployment and isolation

### Game 
```

    Classic Pong gameplay (with a twist in multiplayer mode)
    Local multiplayer (same keyboard)
    Tournament system with automatic matchmaking
    Match history stored and displayed in main user's profile
    Babylon.js used for game rendering
```

### User & Social

    User registration and authentication
    JWT-based authentication
    Two-Factor Authentication (2FA)
    Profile management and customization
    Add and manage friends

### Security

    Password hashing
    Strict password requirements
    Secure API routes
    Input validation in both frontend and backend
    HTTPS

### Technical Requirements

    Single page application
    Compatible with the latest Mozilla Firefox and expanded browser compatibility
    No unhandled runtime errors or warnings
    Fully containerized with Docker (single command setup)

