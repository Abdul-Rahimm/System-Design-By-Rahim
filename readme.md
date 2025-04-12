# Knowledge Vault

A simple, decoupled web archive to store and browse articles and videos categorized by subject — System Design, LeetCode, DevOps, and more.

---

## ✨ Features

- Clean two-column layout:
  - Left: Article thumbnails
  - Right: Video thumbnails
- Clicking an article opens a full article view
- Clicking a video opens the YouTube video in a new tab
- Fully decoupled architecture: Backend (Go) and Frontend (Next.js) communicate via REST APIs
- Easily extendable to other subjects and content types

---

## 🚀 Tech Stack

| Layer      | Technology        |
|------------|-------------------|
| Frontend   | Next.js, React    |
| Backend    | Go (Golang)       |
| API        | REST (JSON)       |
| Styling    | TailwindCSS (optional) |
| Hosting    | Vercel / Netlify (Frontend), Render / Fly.io (Backend) |

---

## 📚 Subjects

Each subject (e.g., `System Design`, `LeetCode`, `DevOps`) will have:

- A list of related **articles** (thumbnail + title + slug + full content)
- A list of related **videos** (thumbnail + title + YouTube URL)

Content is fetched dynamically via REST APIs and rendered on the frontend.

---

## 🔄 Project Structure

```
/knowledge-vault
├── backend/              # Go REST API
│   ├── main.go
│   ├── handlers/
│   ├── models/
│   └── storage/
└── frontend/             # Next.js app
    ├── pages/
    ├── components/
    └── lib/
```

---

## 🔧 Getting Started

### Backend (Go API)
```bash
cd backend
# install Go dependencies (if any)
go run main.go
# Server will run on http://localhost:8080
```

### Frontend (Next.js)
```bash
cd frontend
npm install
npm run dev
# App runs on http://localhost:3000
```

---

## 🔗 API Endpoints

| Method | Endpoint                | Description               |
|--------|-------------------------|---------------------------|
| GET    | /api/articles           | List all articles         |
| GET    | /api/articles/{slug}    | Get article by slug       |
| GET    | /api/videos             | List all videos           |

---

## 📆 Future Enhancements

- Admin panel to manage content
- Search and filter by tag or subject
- Pagination and lazy loading
- Markdown support for articles
- GitHub integration to pull article repos

---

## 🌟 License

MIT License

---

## 👤 Author

Built with ❤️ by Abdul Rahim· Inspired by the need to organize learning materials efficiently.

