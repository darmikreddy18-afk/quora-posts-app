# 📝 REST Posts App

A simple **CRUD (Create, Read, Update, Delete)** web application built using **Node.js, Express, and EJS**.
This project simulates a basic social platform where users can create, view, edit, and manage posts.

---

## 🚀 Features

* ➕ Create a new post
* 📄 View all posts
* 🔍 View a single post
* ✏️ Edit existing post
* 🧠 RESTful routing structure
* 🔁 Method override for PATCH requests

---

## 🛠️ Tech Stack

* **Node.js** – Runtime environment
* **Express.js** – Backend framework
* **EJS** – Templating engine
* **UUID** – Unique ID generation
* **method-override** – Enable PATCH/DELETE from forms
* **CSS** – Basic styling

---

## 📂 Project Structure

```
REST_CLASS/
│
├── views/         # EJS templates (index, create, edit, show)
├── public/        # Static files (CSS)
├── node_modules/  # Dependencies (ignored)
├── index.js       # Main server file
├── package.json
├── .gitignore
└── README.md
```

---

## 🔄 CRUD Operations Explained

### ➕ Create (POST)

* Route: `/posts`
* Adds a new post with `username` and `content`

---

### 📄 Read (GET)

* `/posts` → View all posts
* `/posts/:id` → View a single post

---

### ✏️ Update (PATCH)

* Route: `/posts/:id`
* Updates the content of an existing post
* Uses `method-override` to simulate PATCH requests

---

### ❌ Delete (Optional Extension)

* Can be implemented using `DELETE /posts/:id`

---

## 🔁 Method Override

Since HTML forms only support GET and POST, this project uses:

```
?_method=PATCH
```

This allows Express to treat POST requests as PATCH requests for updating data.

---

## ⚙️ Installation & Setup

1. Clone the repository:

```
git clone https://github.com/darmikreddy18-afk/quora-posts-app.git
```

2. Navigate into the folder:

```
cd rest-posts-app
```

3. Install dependencies:

```
npm install
```

4. Run the server:

```
node index.js
```

5. Open in browser:

```
http://localhost:8080/posts
```

---

## 🧠 Key Learnings

* Understanding RESTful routing
* Difference between POST and PATCH
* Handling form data with `req.body`
* Using `req.params` vs `req.query`
* Dynamic routing in Express
* Server-side rendering with EJS

---

## 📌 Future Improvements

* 🗑️ Add delete functionality
* ❤️ Add like feature
* 🗃️ Connect to a database (MongoDB)
* 🔐 Add authentication
* 🎨 Improve UI/UX

---

## 👨‍💻 Author

**Darmik Reddy**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
