# 📝 NoteKeeper API

A **NestJS-based backend** for a smart, modular note-taking application. Supports full CRUD for notes, tagging, scheduled reminders, and powerful REST APIs. Built for extensibility, performance, and future integration with web & mobile frontends.

---

## 📦 Tech Stack

- **Backend Framework**: [NestJS](https://nestjs.com/)
- **Database**: PostgreSQL (via Drizzle)
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

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | /notes         | Get all notes |
| POST   | /notes         | Create a new note |
| GET    | /notes/:id     | Get a note by ID |
| PATCH  | /notes/:id     | Update a note |
| DELETE | /notes/:id     | Delete a note |
| GET    | /reminders/today | Get today's reminders |
| GET    | /notes?tag=work | Filter by tag |

---

## 🛠 Setup Instructions

```bash
# Clone repo
git clone https://github.com/yourusername/notekeeper-api.git
cd notekeeper-api

# Install dependencies
npm install

# Start Postgres locally or via Docker
# Create a .env file (see below)

# Run the app
npm run start:dev

# Swagger Docs
# Visit http://localhost:3000/api
PORT=3000
DB_HOST=localhost
DB_PORT=5432
DB_USERNAME=postgres
DB_PASSWORD=postgres
DB_NAME=notekeeper
JWT_SECRET=supersecret

---

## ✅ Next Steps:

1. Create a repo: `NoteKeeper-API`
2. Add this as `README.md`
3. Initialize the NestJS app:
```bash
nest new notekeeper-api
