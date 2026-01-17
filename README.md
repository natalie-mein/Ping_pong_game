# FT_TRANSCENDENCE

<p align="center" width="100%">
    <img width="33%" src="https://github.com/natalie-mein/images/blob/main/ft_transcendencem.png">
</p>

## Project Overview

Ft_transcendence is a full-stack web application and multiplayer gaming platform built as part of the 42 curriculum.
The project combines real-time gameplay, user management, and tournament features while following a microservices architecture with secure authentication.
Players can compete in a classic Pong game against friends, or random opponents, and managing their profiles.
Key Features

🎮 Real-time Pong Gameplay – Play against humans or AI opponents.
🧑‍🤝‍🧑 User Management – Registration, login, and profile customization.
🔐 Secure Authentication – JWT-based login and Two-Factor Authentication (2FA).
🏆 Tournaments – Organize and participate in competitive tournaments.
🌐 Multi-language Support – Accessibility for diverse users.
🐳 Containerized Deployment – Fully managed with Docker Compose.
Tech Stack

Frontend

    React – Component-based UI
    TypeScript – Type-safe development
    Tailwind CSS – Utility-first styling

Backend & Architecture

    Node.js + Fastify – High-performance backend services
    Microservices Architecture – Modular design for scalability
    SQLite – Lightweight database for persistence
    Sequelize – ORM for structured and maintainable database management
    WebSockets – Real-time communication
    Docker & Docker Compose – Simplified deployment and isolation

How to run

    Clone the project

git clone https://github.com/Sherry5Wu/ft_trancedence.git ft_trancedence && cd ft_trancedence

    This project uses a .env file to store sensitive configuration values such as authentication secrets, API keys, and database paths.
    Here are steps for prepare your own .env files.
    Copy .env.example to .env

cp ./services/auth-service/.env.example ./services/auth-service/.env

Fill in your own values Open the .env file and replace the placeholder values with your own credentials or secrets. For example:

#jwt_secret_key (32+)
JWT_SECRET=your-jwt-secret-here (32+ characters)
JWT_REFRESH_SECRET=your-refresh-secret-here

# 2fa encryption key
TWOFA_ENC_KEY=your-2fa-encryption-key-here

# Google sign in
GOOGLE_CLIENT_ID=your-client-id
GOOGLE_CLIENT_SECRET=your-client-secret

The backend automatically reads the variables from your .env file. Make sure the values are valid; otherwise, authentication and database connections may fail.

    Build the containers up

make

please be patient, this step may take around 2~3 minutes.

    After all the services(containers) are up, then you can access to the website: https://localhost:8443
    Because the website uses a self-signed certificate, you will see the warning page shown below.
    Don’t worry — just click “Advanced”, then click “Proceed to localhost (unsafe)”.
    Note: I used Google Chrome, so if you are using a different browser, the wording may be slightly different.
