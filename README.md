# TDS Project 1

## Getting Started

### 1. Clone the Repository
```sh
git clone https://github.com/your-username/tdsproject1.git
cd tdsproject1
```

---

### 2. Build or Pull the Docker Image

#### Option A: Build from Source
```sh
docker build -t nashiitm/tdsproject1 .
```

#### Option B: Pull from Docker Hub
```sh
docker pull docker.io/nashiitm/tdsproject1
```

---

### 3. Run the Docker Container
Replace `your_actual_token` with your actual AI proxy token:
```sh
docker run -e AIPROXY_TOKEN=your_actual_token -p 8000:8000 nashiitm/tdsproject1:latest
```

---

### 4. Running `evaluate.py`
To evaluate, use:
```sh
uv run evaluate.py --email=your@email.com --log-level=INFO
```

---

### 5. Ensure Data Folder is Generated
- The `data` folder should be generated from `datagen.py`.
- If the folder is missing, run:
  ```sh
  python datagen.py
  ```
  to create the necessary data.

---

### 6. File Structure
For best results, ensure that the following files are in the same directory:
- `datagen.py`
- `evaluate.py`
- `.env`

---

### Notes
- Double-check dependencies and environment variables before running.
- If you encounter issues, ensure all required Python packages are installed.

---

Thanks for using **TDS Project 1**! 🚀
