# Prompt-Powered Kickstart: Building a Beginner’s Toolkit for FastAPI

---

## 1. Overview of the Technology

### What is FastAPI?
FastAPI is a modern Python web framework used to build APIs quickly and efficiently. It is designed for high performance and simplicity.

### Why FastAPI?
- Easy to learn for beginners  
- Fast performance  
- Built-in API documentation  
- Suitable for backend and data-driven applications  

### Use Cases
- Backend services  
- REST APIs  
- Data and machine learning model deployment  

---

## 2. Setup Instructions

### System Requirements
- Python 3.7 or higher  
- VS Code  
- Terminal (Command Prompt / VS Code terminal)

---

### Step-by-Step Installation

#### 1. Create Project Folder
```
mkdir fastapi-toolkit
cd fastapi-toolkit
```

#### 2. (Optional) Create Virtual Environment
```
python -m venv venv
```

Activate:

Windows:
```
venv\Scripts\activate
```

Mac/Linux:
```
source venv/bin/activate
```

#### 3. Install Dependencies
```
pip install fastapi uvicorn
```

---

## 3. Minimal Working Example

### File: main.py

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def home():
    return {"message": "Welcome to FastAPI Toolkit"}

@app.get("/about")
def about():
    return {"info": "This project demonstrates FastAPI basics"}

@app.get("/user/{name}")
def get_user(name: str):
    return {"user": name, "message": f"Hello {name}"}
```

---

### Run the Application
```
uvicorn main:app --reload
```

---

### Access in Browser
- http://127.0.0.1:8000  
- http://127.0.0.1:8000/docs  

---

## 4. AI Prompts Used & Learning Reflection

### AI Prompts Used

| Prompt | Purpose | Outcome |
|------|--------|--------|
| What is FastAPI? | Understanding concept | Learned API basics |
| How to install FastAPI in VS Code? | Setup | Installed dependencies |
| Create a simple FastAPI app | Development | Built working API |
| Fix SyntaxError when running uvicorn | Debugging | Resolved issue |

### Learning Reflection

This project demonstrates how generative AI (via ai.moringaschool.com) can support beginner learning in software development.

AI was used to:
- Understand new concepts quickly  
- Generate starter code  
- Debug errors efficiently  
- Improve project structure  

---

## 5. Common Errors & Solutions

| Error | Cause | Solution |
|------|------|---------|
| SyntaxError when running uvicorn | Running command inside Python | Run in terminal |
| ModuleNotFoundError: fastapi | Package not installed | pip install fastapi uvicorn |
| Port already in use | Another app running | Change port to 8001 |
| Command not recognized | Uvicorn not in PATH | Use python -m uvicorn |

---

## 6. Reference Resources

- https://fastapi.tiangolo.com  
- https://docs.python.org  
- https://www.uvicorn.org  
- https://www.w3schools.com  

---

## 7. How to Run the Project

```
git clone <your-repo-link>
cd fastapi-toolkit
pip install fastapi uvicorn
uvicorn main:app --reload
```

---

## 8. Working Codebase

Upload this project to GitHub and include:
- main.py  
- README.md  

---

## Final Note

This project demonstrates how AI can accelerate learning, simplify debugging, and improve development efficiency for beginners.
# Technology-Chosen-FastAPI-Python-Framework-
