
# 🌾 Farmer-Hub

Farmer-Hub is a full-stack web application designed to support farmers with a powerful platform combining a FastAPI backend and a modern React frontend using Vite and ShadCN UI components.

---

## 🧱 Tech Stack

- **Frontend**: React, Vite, JavaScript, TypeScript, Tailwind CSS, ShadCN/UI
- **Backend**: FastAPI, Uvicorn
- **Other**: Python virtual environment, dotenv for environment config, multipart/form-data support

---

## 📁 Folder Structure

```
Farmer-Hub/
├── backend/        # FastAPI backend
├── frontend/       # React frontend (Vite + Tailwind + ShadCN)
└── README.md       # Project documentation
```

---

## ⚙️ Backend Setup (FastAPI)

### 1. Navigate to backend

```bash
cd backend
```

### 2. Create and activate virtual environment

```bash
python -m venv myenv
myenv\Scripts\activate  # Windows
```

### 3. Install backend dependencies

```bash
pip install fastapi uvicorn python-dotenv python-multipart
```

> Optional: Create a `requirements.txt` with:
> ```
> fastapi
> uvicorn
> python-dotenv
> python-multipart
> ```

### 4. Create `.env` file

Add environment variables as needed (e.g., for database, cloud storage, etc.):


```env
EXAMPLE_KEY=value
DATABASE_URL=your_database_url
```

### 5. Run the FastAPI server

```bash
uvicorn main1:app --reload
```

- Swagger Docs: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

---

## 💻 Frontend Setup (React + Vite + ShadCN)

### 1. Navigate to frontend

```bash
cd ../frontend
```

### 2. Install frontend dependencies

```bash
npm install
```

### 3. Run the frontend development server

```bash
npm run dev
```

- Local: [http://localhost:8080](http://localhost:8080)
- Network: Available at your local IP (for testing on other devices)

---

## 🛠 Common Fixes

- **Form Data Error in FastAPI**:  
  Install: `pip install python-multipart`

- **Missing dotenv**:  
  Install: `pip install python-dotenv`

- **Browserslist warning in React**:
  ```bash
  npx update-browserslist-db@latest
  ```

- **Audit & Fix Node Vulnerabilities**:
  ```bash
  npm audit fix
  ```

---

## 🤝 Contributing

Feel free to fork, suggest changes, or raise issues!

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
