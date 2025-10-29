# 🧭 Employee Directory With Search

## 📌 Project Overview
The **Employee Directory With Search** is a full-stack web application designed to help organizations **store, manage, and search employee details efficiently**.  
It provides a clean and responsive interface where users can search employees by name, department, or designation — improving communication and collaboration within the organization.  

This project was developed as part of the **Naan Mudhalvan Training Program** at *Grace College of Engineering* (CSE Department).

---

## 👥 Team Members
| Name | Register Number |
|------|------------------|
| Princy Shekkinah P | 950323104059 |
| Ramya Mathu Mathi K | 950323104061 |
| Sahaya Merlin A | 950323104063 |
| Selvi P | 950323104066 |

**Trainer:** Ragunath R  
**College Code:** 9503  

---

## 🚀 Features
✅ Add, update, and delete employee records  
✅ Real-time search by name, department, or designation  
✅ RESTful API integration between frontend and backend  
✅ Role-based access and validation  
✅ Responsive and mobile-friendly design  
✅ Secure with data validation and encryption  
✅ Export employee data for reports  

---

## 🧩 Tech Stack

### **Frontend:**
- React.js (for UI rendering)
- Axios (for API communication)
- HTML5, CSS3, JavaScript (for responsive design)

### **Backend:**
- Node.js
- Express.js
- MongoDB (NoSQL database)

### **Testing & Tools:**
- Jest & Supertest (API testing)
- Docker (optional deployment)
- GitHub (version control)

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/employee-directory-with-search.git
cd employee-directory-with-search
```

### 2️⃣ Setup Backend
```bash
cd backend
npm install
```

Create a `.env` file:
```
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/employeeDB
```

Start the backend server:
```bash
npm run dev
```
Server will run on: [http://localhost:5000](http://localhost:5000)

---

### 3️⃣ Setup Frontend
```bash
cd frontend
npm install
npm start
```
Frontend runs on [http://localhost:3000](http://localhost:3000)

---

### 4️⃣ Run with Docker (Optional)
```bash
docker-compose up --build
```

This starts MongoDB, backend, and frontend together.

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|---------|-----------|--------------|
| **GET** | `/api/employees` | Get all employees or search using `?q=` query |
| **POST** | `/api/employees` | Add a new employee |
| **GET** | `/api/employees/:id` | Get a single employee by ID |
| **PUT** | `/api/employees/:id` | Update employee details |
| **DELETE** | `/api/employees/:id` | Delete employee record |

**Example Request:**
```json
POST /api/employees
{
  "name": "Alice Johnson",
  "email": "alice@example.com",
  "department": "HR",
  "role": "Manager",
  "phone": "9876543210"
}
```

---

## 🧠 How It Works
1. Users interact with the React frontend to view or search employees.  
2. React sends API requests to the Node.js backend via Axios.  
3. The backend connects to MongoDB to retrieve or store data.  
4. Results are returned as JSON and displayed dynamically.  

---

## 🧪 Testing
To test the API endpoints:
```bash
cd backend
npm test
```
This runs Jest + Supertest for automated backend testing.

---

## 📷 Screenshots
*(Attach these before final submission)*  
- Homepage showing employee list  
- Search bar in action  
- Employee profile view  
- Postman API test result  
- MongoDB data view  

---

## 💡 Challenges & Solutions
| Challenge | Solution |
|------------|-----------|
| Handling real-time search | Used MongoDB regex with case-insensitive queries. |
| Data validation | Implemented `express-validator` in backend. |
| CORS errors between React & Node | Added CORS middleware in Express. |
| Deployment on cloud | Dockerized backend + frontend for easier hosting. |

---

## 🌐 Deployment
You can deploy this project using:
- **Frontend:** Vercel or Netlify
- **Backend + DB:** Render or Railway (MongoDB Atlas for database)

**Example:**
- Frontend: https://employee-directory-demo.vercel.app
- Backend API: https://employee-directory-api.onrender.com/api/employees

---

## 🏁 Conclusion
The **Employee Directory With Search** successfully integrates React, Node.js, and MongoDB to deliver a modern, scalable employee management system.  
It simplifies internal communication, improves productivity, and demonstrates core full-stack development skills.
