# 🏠 Floor Plan Optimizer

[![GitHub Repo](https://img.shields.io/badge/GitHub-Floor_Plan_Optimizer-blue?logo=github)](https://github.com/RithyaLB/Floor_Plan_Optimizer)

Floor Plan Optimizer is a tool that takes a **floor plan image** as input and evaluates it based on architectural design principles. It scores each room and the overall layout on criteria such as **space utilization**, **lighting and ventilation**, **accessibility**, and **functional layout**. Additionally, it provides **recommendations** for improvements.

---

## 🔍 Features

- 📷 Upload **floor plan images**.
- 🔍 **OCR (PyTesseract)** to detect room names and boundaries.
- 📏 Compute **area**, **room count**, and **number of windows**.
- 🧠 With the **number of occupants** and match against standards.
- 🧾 Scoring system based on:
  - Space utilization
  - Natural lighting and ventilation
  - Accessibility
  - Functional layout
- 🛠 Suggestions based on architectural best practices.
- 🖼️ Visual output: annotated floor plans with scores and feedback.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/RithyaLB/Floor_Plan_Optimizer.git
cd Floor_Plan_Optimizer
```

### 2. Set Up the Environment

Create and activate a virtual environment:

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 📁 Project Structure

```
Floor_Plan_Optimizer/
│
├── backend/
│   ├── app.py                     # Flask backend server
│   └── ideal_room_area_per_person_with_windows.csv  # Architecture standards
│
├── UploadUI.HTML                 # Frontend HTML file (UI)
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

---

## 🏃‍♂️ Running the App

1. **Start the Flask backend:**

```bash
cd backend
python app.py
```

2. **Launch the frontend:**

- Open `UploadUI.HTML` in your browser.

3. **Interact with the App:**

- Upload a floor plan image.
- Select the number of occupants.
- View room-wise and overall scores with recommendations.
- Output visuals will be generated and displayed.

---

## 🧠 Output and Visualizations

- Annotated floor plan with detected rooms and boundaries.
- Visual indicators of windows and area.
- Scorecards for each room and total floor plan.
- Textual suggestions to improve design.

---

## 🧾 Architecture Standards

- Stored in: `backend/ideal_room_area_per_person_with_windows.csv`
- Contains room size, occupant standards, and window requirements.
