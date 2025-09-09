# 📚 Book Social Network

## 📖 Description
**Book Social Network** is a full-stack application that allows users to manage their book collections and interact with a community of book lovers.  
Users can add books, categorize them, and share reviews with other members.

---

## 🛠️ Technologies Used
- **Frontend**: React.js, HTML5, CSS3
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Dependency Management**: npm
- **Containerization**: Docker (optional)

---

## 📂 Project Structure
```text
book-social-network/
├── backend/
│   ├── controllers/      # API route logic
│   ├── models/           # Database schemas
│   ├── routes/           # API route definitions
│   ├── config/           # DB config and other settings
│   ├── middleware/       # Auth and error handling
│   └── server.js         # Backend entry point
├── frontend/
│   ├── src/
│   │   ├── components/   # React components
│   │   ├── pages/        # Application pages
│   │   ├── services/     # API service calls
│   │   └── App.js        # Main React component
│   ├── public/
│   │   └── index.html    # Main HTML file
│   └── package.json      # Frontend dependencies and scripts
├── .gitignore
├── docker-compose.yml    # Docker configuration (optional)
└── README.md
```

---

## 🚀 Installation

### Prerequisites
- Node.js v14+
- npm v6+
- MongoDB (local or Atlas)

### Steps
1. Clone the repository:
```bash
git clone https://github.com/ines5101998/book-social-network.git
cd book-social-network
```

2. Install backend dependencies:
```bash
cd backend
npm install
```

3. Configure your database in `backend/config/db.js` with your MongoDB URL.

4. Start the backend server:
```bash
npm start
```

5. Install frontend dependencies:
```bash
cd ../frontend
npm install
```

6. Start the frontend application:
```bash
npm start
```

Access the app at: [http://localhost:3000](http://localhost:3000)

---

## 🔧 Usage Examples

### Add a Book
```http
POST /api/books
{
  "title": "Le Petit Prince",
  "author": "Antoine de Saint-Exupéry",
  "genre": "Fiction",
  "description": "A poetic and philosophical tale."
}
```

### Get All Books
```http
GET /api/books
```

### Register User
```http
POST /api/users/register
{
  "username": "john_doe",
  "email": "john@example.com",
  "password": "password123"
}
```

### Login User
```http
POST /api/users/login
{
  "email": "john@example.com",
  "password": "password123"
}
```

---

## 🧪 Testing
1. Install test dependencies:
```bash
npm install --save-dev jest
```

2. Add test script in `package.json`:
```json
"scripts": {
  "test": "jest"
}
```

3. Create test files under `backend/tests/`.

4. Run tests:
```bash
npm test
```

---

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch:
```bash
git checkout -b feature/your-feature
```
3. Commit changes:
```bash
git commit -am "Add new feature"
```
4. Push to branch:
```bash
git push origin feature/your-feature
```
5. Open a Pull Request

---

## 📜 License
This project is licensed under the **MIT License**.
