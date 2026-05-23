# SMP Web App — Backend

RESTful API backend for the SMP Web App, developed for [Saturday Morning Physics](https://www.iap.tu-darmstadt.de/smp/saturday_morning_physics/index.de.jsp) at TU Darmstadt. Built as part of the Software Development Project course (2025) in a team of 5.

## Features

- JWT authentication and role-based authorization (Organizer, Participant, HiWi)
- QR code-based attendance validation
- Event lifecycle management with registration approval workflows
- RESTful API for session management, registrations, and attendance tracking
- Dockerized and deployed on a remote server with Nginx

## Tech Stack

Node.js · Express · TypeScript · Prisma · PostgreSQL · Docker · Nginx

## Setup

1. `npm install`
2. `cp .env.example .env` — fill in your DB credentials
3. `createdb smp_dev`
4. `npx prisma migrate dev`
5. `npm run dev` → runs on http://localhost:3000
