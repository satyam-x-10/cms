# 🐍 Simple CMS (`cms-lab`) - Python Flask & MongoDB

A server-side rendered Blog Content Management System built with **Python, Flask, PyMongo, and Jinja2 Templates** according to the **Backend Development Lab Examination** specifications.

---

## 📁 Exact Directory Structure

```text
cms-lab/
├── app.py                # Flask entry point
├── templates/
│   ├── posts.html        # List of posts
│   ├── new-post.html     # Create-post form
│   └── post.html         # Individual post
└── static/
    └── style.css         # Modern glassmorphism CSS
```

---

## ⚡ How to Open & Run in VS Code

### Step 1: Open in VS Code
1. Open **Visual Studio Code**.
2. Click **File > Open Folder...** and select `C:\Users\91895\Desktop\cms-lab`.

### Step 2: Install Dependencies & Run
Open the terminal in VS Code (`Ctrl + ~`) and run:

```bash
pip install -r requirements.txt
python app.py
```

### Step 3: View in Browser
- **Post List**: [http://127.0.0.1:5000/posts](http://127.0.0.1:5000/posts)
- **Create Post**: [http://127.0.0.1:5000/posts/new](http://127.0.0.1:5000/posts/new)

---

## 📝 Compulsory Requirements Checklist

| Requirement | Status | Details |
| :--- | :---: | :--- |
| **1. Display All Posts (`GET /posts`)** | ✅ | Displays post Title (clickable link), Author, and Creation Date. Full content body is excluded from query. |
| **2. Create Post (`POST /posts`)** | ✅ | Form with Title, Author, Content. Automatically generates timestamp on Flask server. Validates non-empty fields and redirects to list. |
| **3. View Individual Post (`GET /posts/<id>`)** | ✅ | Retrieves complete post document by `ObjectId(id)` from MongoDB and displays full content. |
| **4. Server-Side Templates** | ✅ | Jinja2 templates (`posts.html`, `new-post.html`, `post.html`). |
| **5. MongoDB Persistence** | ✅ | Connects to MongoDB `cms_lab` database via PyMongo. Data persists across server restarts. |
