# 🚀 Start FastAPI Backend for Full ML Predictions

## Quick Setup (5 minutes):

### 1. Install Python Dependencies
```bash
cd backend
pip install fastapi uvicorn pandas numpy scikit-learn joblib pydantic requests
```

### 2. Train ML Models
```bash
python train_models.py
```
**Output:** Creates `models/` folder with trained ML models

### 3. Start FastAPI Server
```bash
python main.py
```
**Output:** Server runs on http://localhost:8000

### 4. Test API
Open browser: http://localhost:8000/docs
You'll see interactive API documentation

## ✅ Verification:
- Dashboard will automatically detect FastAPI backend
- You'll get advanced ML predictions instead of fallback
- Real weather API integration
- Historical data storage in SQLite

## 🔧 Troubleshooting:

**Error: "Module not found"**
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

**Error: "Port already in use"**
```bash
# Kill process on port 8000
netstat -ano | findstr :8000
taskkill /PID <PID_NUMBER> /F
```

**Error: "Models not found"**
```bash
# Make sure you ran training first
python train_models.py
# Check if models/ folder exists with .pkl files
```

## 🎯 What You Get:
- **Real ML Models**: Trained RandomForest algorithms
- **Weather Integration**: Live weather API data
- **Database Storage**: SQLite with historical tracking
- **Advanced Insights**: Personalized recommendations
- **Performance Metrics**: R² > 0.8 model accuracy