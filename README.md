# 📝 Blog API & CRUD Application  
A simple full-stack blog application built using **Node.js**, **Express.js**, **EJS**, and **Axios**.  
This project demonstrates CRUD operations, routing, template rendering, REST API creation, and state management using an **in-memory datastore**.

---

## 🚀 Features
- ✅ Full CRUD Blog System  
- ✅ Create, Read, Update, Delete blog posts  
- ✅ Express-based REST API (PORT 4000)  
- ✅ Frontend rendered using EJS Templates (PORT 3000)  
- ✅ In-memory datastore to store posts  
- ✅ Modular routing and clean API structure  
- ✅ Simple UI for adding/editing posts  

---

## 🛠️ Tech Stack
**Backend:**
- Node.js  
- Express.js  
- Body-Parser  
- Axios  

**Frontend:**
- EJS Templates  
- HTML / CSS  

---
```
## 📁 Project Structure
│
├── index.js # REST API (CRUD operations)
├── server.js # Frontend server rendering EJS views
├── views/ # EJS templates
│ ├── index.ejs
│ └── modify.ejs
├── public/
│ └── styles/main.css
├── package.json
└── README.md
```



---

## 🔌 API Endpoints (index.js)
### **GET /posts**
Fetch all blog posts.

### **GET /posts/:id**
Fetch a blog post by ID.

### **POST /posts**
Create a new blog post.  
Body:
```json
{
  "title": "My Post",
  "content": "Post details...",
  "author": "Komal"
}
```

###  **PATCH /posts/:id**

Update one or more fields of an existing post.

### **DELETE /posts/:id**
Delete a post by ID.



## 💻 Frontend Routes (server.js)

### **GET /**
Renders home page and lists all posts.

### **GET /new**
Page to create a new post.

### **GET /edit/:id**
Page to edit an existing post.

### **POST /api/posts**
Create a new post via API.

### **POST /api/posts/:id**
Update a post via API.

### **GET /api/posts/delete/:id**
Delete a post via API.

---

## ▶️ How to Run Locally

- ✅ Install dependencies
```
npm install
```

- ✅ Start the API Server (PORT 4000)
```
node index.js
```

- ✅ Start the Frontend Server (PORT 3000)
Open a new terminal:
```
node server.js
```

- Now visit:
👉 http://localhost:3000

---

## 📌 Notes

This project uses an in-memory datastore, so posts are not persistent.
When the server restarts, all added posts reset.

This makes the project lightweight and perfect for understanding CRUD + Express basics.

---


## ⭐ Future Enhancements

🔹 Add database support (MongoDB / PostgreSQL)

🔹 Add user authentication

🔹 Add validation & error handling

🔹 Deploy frontend & backend separately

🔹 Add edit/delete confirmation dialogs

---


## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to modify.

---


## 🧑‍💻 Author

Komal Baid
Portfolio: https://www.komalbaid.in
