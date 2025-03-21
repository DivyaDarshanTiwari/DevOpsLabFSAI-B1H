# LAB-6

## Author

1. Name- Divya Darshan Tiwari
2. SAP- 500105299
3. Roll No. - R2142220070
4. Batch - B1H Full Stack AI

---

## Steps to Set Up FastAPI with Docker

### 1. Open WSL

wsl

### 2. Install Python

sudo apt install python3-pip -y

### 3. Install FastAPI and Uvicorn

pipenv install fastapi uvicorn

### 4. Open Visual Studio Code (through Ubuntu)

code .

### 5. Create a Project Directory and Necessary Files

#### main.py

from fastapi import FastAPI
import uvicorn # Ensure you have uvicorn installed

app = FastAPI()

@app.get("/")
def read_root():
return dict(name="Divya", Location="Dehradun")

@app.get("/{data}")
def read_root(data):
return dict(hi=data, Location="Dehradun")

if **name** == "**main**":
uvicorn.run("main:app", host="0.0.0.0", port=8000, reload = True)

#### requirements.txt

fastapi
uvicorn

#### Dockerfile

FROM ubuntu

RUN apt update -y
RUN apt install python3 python3-pip pipenv -y

WORKDIR /app
COPY . /app/
RUN pipenv install -r requirements.txt

EXPOSE 8000

CMD pipenv run python3 ./main.py

### 6. Build Docker Image

docker build -t test .

### 7. Verify Docker Image Creation

docker images

### 8. Run the Docker Image

docker run -p 8000:8080 a03825

Output in terminal:
INFO: Will watch for changes in these directories: ['/app']
INFO: Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
INFO: Started reloader process [7] using StatReload
INFO: Started server process [10]
INFO: Waiting for application startup.
INFO: Application startup complete.
