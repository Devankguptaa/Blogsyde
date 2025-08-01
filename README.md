# 📝 MERN Blog Platform

A full-stack blogging platform built using the **MERN** stack (MongoDB, Express.js, React.js, Node.js). Users can register, log in, create blog posts with images, edit posts, and view all recent blogs. This project uses **JWT authentication**, **cookie-based sessions**, and supports **file uploads** with `multer`.

---

## 🚀 Features

- 🔐 User Registration, Login, Logout (JWT + Cookies)
- 📝 Create, Edit, Delete Blog Posts
- 📚 View All Posts & Individual Post Pages
- 🖼️ Upload Cover Images (handled via Multer)
- ⏱️ Post Timestamps with Mongoose
- 🧾 Rich Text Editor support (React Quill)
- 🗃️ Author-based post filtering

---

## 🛠️ Tech Stack

| Category    | Tech                  |
|-------------|------------------------|
| Frontend    | React.js, React Quill |
| Backend     | Node.js, Express.js   |
| Database    | MongoDB + Mongoose    |
| Auth        | JWT, bcryptjs, cookie-parser |
| File Upload | Multer                |

---

## 📁 Project Structure

```
mern-blog-master/
├── api/                  # Backend - Express App
│   ├── models/           # Mongoose Schemas (User, Post)
│   └── index.js          # Server and Routes
├── client/               # Frontend - React App
│   ├── public/           # Static files
│   └── src/              # React Components
```

---

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/mern-blog.git
cd mern-blog-master
```

---

### 2. Backend Setup (`api/`)

```bash
cd api
npm install
```

🔐 Create a `.env` file in the `api/` folder:

```
MONGO_URL=your_mongodb_connection_url
JWT_SECRET=your_secret_key
```

Start the backend server:

```bash
node index.js
```

Runs at: [http://localhost:4000](http://localhost:4000)

---

### 3. Frontend Setup (`client/`)

```bash
cd ../client
npm install
npm start
```

Runs at: [http://localhost:3000](http://localhost:3000)

---

## 🔧 API Routes Overview

| Route             | Method | Description           |
|------------------|--------|-----------------------|
| `/register`       | POST   | Register new user     |
| `/login`          | POST   | Login user            |
| `/logout`         | POST   | Logout user           |
| `/profile`        | GET    | Get logged-in profile |
| `/post`           | POST   | Create new post       |
| `/post`           | PUT    | Edit existing post    |
| `/post`           | GET    | Get all posts         |
| `/post/:id`       | GET    | Get post by ID        |

---



## 🌐 Deployment (Recommended)

- Frontend: [Vercel](https://vercel.com/)
- Backend: [Render](https://render.com/)
- Database: [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)

---

## 💡 Future Enhancements

- 🔎 Search & Pagination
- 💬 Comments system
- 📱 Responsive mobile UI
- 🔐 Role-based admin panel
- ☁️ Cloudinary integration for image storage

---

## 📄 License

MIT License - Feel free to use and modify ✌️

---

## 🙌 Acknowledgements

- [React](https://reactjs.org/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://mongodb.com/)
- [Multer](https://github.com/expressjs/multer)
- [React Quill](https://github.com/zenoamaro/react-quill)
