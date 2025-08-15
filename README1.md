# 🦷 Dental Cavity Detection Web App

A full-stack web application that detects **dental cavities** from uploaded teeth images using a YOLOv8 deep learning model. Designed for educational and demo purposes, this app enables users to input patient details, upload dental images, and receive real-time cavity detection results with annotated visuals.

---

## ✅ Key Features

- 📤 Upload patient name, age, and dental image  
- 🖼️ Real-time image preview before submission  
- 🧠 Cavity detection using YOLOv8 model  
- 📊 Display cavity count and annotated result image  
- 🌐 Full-stack architecture: Node.js backend + Python model + HTML/CSS/JS frontend  

---

## 📁 Project Structure

### 🌐 Frontend

Built with static HTML, CSS, and JavaScript:

| File         | Description |
|--------------|-------------|
| `index.html` | Form for patient details and image upload with live preview |
| `report.html`| Displays detection results including cavity count and annotated image |
| `style.css`  | Responsive and clean UI styling |
| `script.js`  | Handles form submission, image preview, and redirection to results |

---

### ⚙️ Backend

Powered by **Node.js + Express**, with Python integration for model inference:

| File         | Description |
|--------------|-------------|
| `app.js`     | Express server that handles uploads, invokes Python detection, and returns JSON |
| `detect.py`  | Loads YOLOv8 model, performs detection, saves annotated image, and returns cavity count |

---

## 🧪 Sample Output

```json
{
  "cavity_count": 3,
  "output_image": "output/result.jpg"
}

🚀 Getting Started
📌 Prerequisites
- Python 3.x
- Required packages: ultralytics, opencv-python
- Node.js (v16+ recommended)
- Trained YOLOv8 model (yolov8.pt in model/ folder)

Setup Instructions
- Install Backend Dependencies
cd backend
npm install
- Install Python Dependencies
pip install ultralytics opencv-python
- Start the Server
node app.js
- Server will run at: http://localhost:5000
- Launch Frontend Open frontend/index.html directly in your browser.

📎 Notes
- Avoid uploading large images to reduce response time.
- Ensure uploads/ and output/ folders have write permissions.
- Exclude node_modules/ from ZIP archives when sharing the project.

👩‍💻 Author
Varshitha Challa
AI Cavity Detection App (2025)
Postgraduate in Artificial Intelligence, KL University.
