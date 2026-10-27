# Project Setup

## 1. Create and activate a Python virtual environment

From the project root:

```powershell
py -3 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

## 2. Install backend dependencies

```powershell
pip install --upgrade pip setuptools wheel
pip install -r backend/requirements.txt
```

## 3. Install frontend dependencies

```powershell
cd frontend
npm install
cd ..
```

## 4. Run the app

### Backend

```powershell
.\.venv\Scripts\python.exe -m uvicorn backend.app.main:app --reload --host 0.0.0.0 --port 8000
```

### Frontend

```powershell
cd frontend

Set-Location 'C:\Users\M VISHNU VARDHAN\OneDrive\Desktop\final\frontend' npm run build
```

The frontend will usually be available at http://localhost:3000 and the backend at http://localhost:8000.
