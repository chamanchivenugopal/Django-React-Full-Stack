# 📂 Full-Stack Notes App
A full-stack web application built using **Django (Backend)** and **React (Frontend)** with **JWT authentication**.

---

## 🚀 Features
- ✅ User Registration & Login with JWT authentication  
- ✅ Secure API for creating, reading, updating, and deleting notes  
- ✅ Protected Routes to restrict access to authenticated users  
- ✅ PostgreSQL as the database  
- ✅ CORS enabled for frontend-backend communication  

---

## 🛠 Tech Stack  
### **Frontend:**
- React.js  
- Vite (Fast build tool)  
- React Router  
- Local Storage for JWT tokens  

### **Backend:**
- Django & Django REST Framework  
- PostgreSQL  
- Simple JWT for authentication  
- CORS Headers  

---

## 📂 Project Structure  
### **Backend (Django)**  
```
backend/
│── api/
│   ├── migrations/
│   ├── models.py  # Database models
│   ├── serializers.py  # API data formatting
│   ├── views.py  # API endpoints
│   ├── urls.py  # API routes
│   ├── admin.py  # Django admin configuration
│   ├── apps.py  # App configuration
│   ├── tests.py  # Unit tests
│── backend/
│   ├── settings.py  # Configuration & Database settings
│   ├── urls.py  # Main URL configuration
│   ├── wsgi.py  # Web Server Gateway Interface
│   ├── asgi.py  # Asynchronous Server Gateway Interface
│── manage.py  # Django command-line tool
│── .env  # Environment variables
│── .gitignore  # Git ignored files
│── Procfile  # Deployment configuration (Heroku)
│── requirements.txt  # Backend dependencies
```

### **Frontend (React + Vite)**  
```
frontend/
│── public/
│── src/
│   ├── assets/  # Static assets (images, icons)
│   ├── components/  # Reusable UI components
│   │   ├── Form.jsx
│   │   ├── LoadingIndicator.jsx
│   │   ├── Note.jsx
│   │   ├── ProtectedRoute.jsx
│   ├── pages/  # Route pages
│   │   ├── Home.jsx
│   │   ├── Login.jsx
│   │   ├── NotFound.jsx
│   │   ├── Register.jsx
│   ├── styles/  # CSS files
│   │   ├── Form.css
│   │   ├── Home.css
│   │   ├── LoadingIndicator.css
│   │   ├── Note.css
│   ├── api.js  # Handles API requests
│   ├── App.jsx  # Main React file with routing
│   ├── constants.js  # Global constants
│   ├── main.jsx  # React entry point
│── .env  # Environment variables
│── .gitignore  # Git ignored files
│── eslint.config.js  # Linting configuration
│── index.html  # Main HTML file
│── package-lock.json  # Dependency lock file
│── package.json  # Frontend dependencies
│── vite.config.js  # Vite configuration
│── README.md  # Project documentation
```

---

## 🌟 Setup & Installation  

### **1. Clone the Repository**  
```sh
git clone https://github.com/chamanchivenugopal/Django-React-Full-Stack
cd fullstack-notes-app
```

### **2. Backend Setup (Django)**  
```sh
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### **3. Frontend Setup (React + Vite)**  
```sh
cd frontend
npm install
npm run dev
```

---

## 🔑 Environment Variables  
Create a `.env` file inside the **backend/** folder:
```env
SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
DataBase_NAME=your_db_name
DataBase_USER=your_db_user
DataBase_PWD=your_db_password
DataBase_HOST=localhost
DataBase_PORT=5432
```

For frontend, create a `.env` file in the **frontend/** folder:
```env
REACT_APP_API_URL=http://localhost:8000/api
```

---

## 💪 API Endpoints  
| Endpoint | Method | Description |
|----------|--------|------------|
| `/api/user/register/` | `POST` | Register a new user |
| `/api/token/` | `POST` | Get access & refresh token |
| `/api/token/refresh/` | `POST` | Refresh expired access token |
| `/api/notes/` | `GET` | Get all notes (Auth required) |
| `/api/notes/` | `POST` | Create a new note |
| `/api/notes/:id/` | `PUT` | Update a note |
| `/api/notes/:id/` | `DELETE` | Delete a note |

---

## 👨‍💻 Contributing  
1. **Fork the repository**  
2. **Create a new branch** (`git checkout -b feature-branch`)  
3. **Commit your changes** (`git commit -m "Added new feature"`)  
4. **Push to the branch** (`git push origin feature-branch`)  
5. **Create a Pull Request**  

---

## 📜 License  
This project is licensed.

---

## 💌 Contact  
For any queries, reach out at:  
📩 Email: chaminchivenugopal@gmail.com 
🔗 GitHub: [chamanchivenugopal](https://github.com/chamanchivenugopal)  

---

🌟 **Happy Coding!** 🌟

