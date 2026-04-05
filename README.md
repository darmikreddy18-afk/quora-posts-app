# 📝 REST Posts App

A full-featured **CRUD (Create, Read, Update, Delete)** web application built using **Node.js, Express, and EJS**.
This project simulates a simple social platform where users can create, view, edit, and delete posts.

---

## 🚀 Features

* ➕ Create a new post
* 📄 View all posts
* 🔍 View a single post
* ✏️ Edit existing post
* 🗑️ Delete a post
* 🔁 RESTful routing using GET, POST, PATCH, DELETE
* ⚙️ Method override for PATCH and DELETE requests

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

```id="hfy54x"
REST_CLASS/
│
├── views/         # EJS templates (index, create, edit, show)
├── public/        # Static files (CSS)
├── index.js       # Main server file
├── package.json
├── .gitignore
└── README.md
```

---

## 🔄 CRUD Operations

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

---

### 🗑️ Delete (DELETE)

* Route: `/posts/:id`
* Removes a post from the list

---

## 🔁 Method Override

Since HTML forms only support GET and POST, this project uses:

```id="cqxjyy"
?_method=PATCH
?_method=DELETE
```

This allows Express to handle PATCH and DELETE requests properly.

---

## ⚙️ Installation & Setup

1. Clone the repository:

```id="b78mbu"
git clone https://github.com/darmikreddy18-afk/quora-posts-app.git
```

2. Navigate into the project folder:

```id="e6gm1y"
cd rest-posts-app
```

3. Install dependencies:

```id="lvhtcu"
npm install
```

4. Run the server:

```id="a3v4dr"
node index.js
```

5. Open in browser:

```id="mbujgc"
http://localhost:8080/posts
```

---

## 🧠 Key Learnings

* Understanding RESTful routing
* Difference between GET, POST, PATCH, DELETE
* Handling form data with `req.body`
* Using `req.params` for dynamic routing
* Method overriding in Express
* Server-side rendering using EJS

---

## 🚀 Future Improvements

* ❤️ Add like functionality
* 🗃️ Connect to a database (MongoDB)
* 🔐 Add user authentication
* 🎨 Improve UI/UX

---

## 👨‍💻 Author

**Darmik Reddy**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!

