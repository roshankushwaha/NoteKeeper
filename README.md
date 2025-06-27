# 📝 NoteKeeper API

A **NestJS-based backend** for a smart, modular note-taking application. Supports full CRUD for notes, tagging, scheduled reminders, and powerful REST APIs. Built for extensibility, performance, and future integration with web & mobile frontends.

---

## 📦 Tech Stack

- **Backend Framework**: [NestJS](https://nestjs.com/)
- **Database ORM**: [Drizzle ORM](https://orm.drizzle.team/)
- **Database**: PostgreSQL
- **Scheduling**: `@nestjs/schedule`
- **Validation**: `class-validator`
- **API Docs**: Swagger
- **Authentication**: JWT (planned)
- **Frontend**: Coming soon (React / React Native)

---

## 🚀 Features

- 🔐 User registration & login (coming soon)
- 🧾 Create, Read, Update, Delete notes
- 🔖 Add tags to notes
- 📅 Add optional reminder timestamps to notes
- 📤 Fetch notes with filters (e.g. by tag or date)
- ⏰ Daily reminder cron job to trigger scheduled notes
- 📘 Swagger API docs auto-generated

---

## 🗂️ Project Structure (Planned)


---

## 📌 API Endpoints Preview

| Method | Endpoint            | Description               |
|--------|---------------------|---------------------------|
| GET    | `/notes`            | Get all notes             |
| POST   | `/notes`            | Create a new note         |
| GET    | `/notes/:id`        | Get a note by ID          |
| PATCH  | `/notes/:id`        | Update a note             |
| DELETE | `/notes/:id`        | Delete a note             |
| GET    | `/reminders/today`  | Get today's reminders     |
| GET    | `/notes?tag=work`   | Filter notes by tag       |

---

## 🛠 Setup Instructions

```bash
# Clone repo
git clone https://github.com/roshankushwaha/notekeeper-api.git
cd notekeeper-api

# Install dependencies
npm install

# Create a .env file (see below)
# Set up PostgreSQL database

# Run migrations using Drizzle
npx drizzle-kit push

# Start the server
npm run start:dev

# Swagger Docs
Visit http://localhost:3000/api
PORT=3000
DATABASE_URL=postgresql://postgres:password@localhost:5432/notekeeper
JWT_SECRET=supersecret

---


Create a new file in your root folder: `LICENSE`

```txt
MIT License

Copyright (c) 2025 Roshan Kushwaha

Permission is hereby granted, free of charge, to any person obtaining a copy...
