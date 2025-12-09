
# 🔐 Safety Path Finder – Women Safety Route Recommender

The **Safety Path Finder** is a web-based application designed to help women identify the safest possible travel routes based on area-wise safety scores. It leverages data science, machine learning, and graph algorithms (BFS) to assist users in avoiding potentially risky paths.

---

## 📌 Table of Contents

- Problem Statement
- Features
- Tech Stack
- How It Works
- Installation
- Usage
- Sample Output
- Future Scope
- Screenshots
- Credits

---

## 🧩 Problem Statement

Incidents like the **Disha case (Hyderabad, 2019)** highlight the importance of **proactive safety solutions**. Women traveling alone often face risks during late hours or through unsafe localities. The project aims to build a tool that helps users choose **safer alternative paths** instead of just the shortest ones.

---

## ⭐ Features

- 🔒 Login system with session tracking
- 🛣️ Route suggestion using **BFS (Breadth-First Search)**
- 📊 Area-wise **safety score analysis**
- 🚦 Risk classification: 🟢 Safe | 🟡 Moderate | 🔴 Risky
- 📁 Input from CSV (safety data) and JSON (route paths)
- 📬 Contact form for feedback
- 🧠 Easy to upgrade with AI/ML models or map integration

---

## 🛠️ Tech Stack

- **Backend**: Python, Flask
- **Frontend**: HTML, CSS, Bootstrap (optional)
- **Data Handling**: Pandas, JSON
- **Routing Algorithm**: BFS (Graph Traversal)
- **Data Storage**: CSV & JSON (currently), can be extended to DB

---

## ⚙️ How It Works

1. **User logs in**
2. Chooses **source** and **destination**
3. All possible paths are found using **BFS**
4. For each path:
   - Safety score is fetched from CSV
   - Average score is calculated
   - Routes are labeled: Safe / Moderate / Risky
5. Safest path is shown to the user with color-coded badge

---

## 🚀 Installation

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/safety-path-finder.git
   cd safety-path-finder
   ```

2. Install dependencies:
   ```bash
   pip install flask pandas
   ```

3. Make sure the following files are in the project folder:
   - `app.py`
   - `templates/` folder with HTML files (index.html, about.html, pathfinder.html, etc.)
   - `static/` folder for styling (optional)
   - `safety_data_updated.csv` (for area-wise safety scores)
   - `all_pincode_paths.json` (for route graph)

4. Run the app:
   ```bash
   python app.py
   ```

5. Open your browser:
   ```
   http://127.0.0.1:5000
   ```

---

## 🧪 Sample Output

- **Best path**: [Shaikpet → Raidurg → Jubilee Hills → Kothaguda → Hitech City]
- **Mean safety score**: 135.6
- **Safety level**: 🟢 Safe

---

## 🔭 Future Scope

- 🔄 Integrate real-time crime data from APIs
- 🗺️ Add map-based route visualization (e.g., Leaflet.js or Google Maps)
- 📲 Make it mobile-friendly or develop a mobile app
- 🧠 Use ML to predict risk based on time of day, weather, past history
- 🧾 Add user registration with database (SQLite, MySQL, etc.)

---

## 📸 Screenshots

## 📸 Screenshots

### 🔐 Login Page
![Login](https://github.com/BinduSundarapu/blob/main/login.png)

### About Page
![About Page](Screenshots/about_safetypath.png)

### 🗺️ Pathfinder Page
![Pathfinder Page](Screenshots/pathfinder.png)

### ✅ Route Output
![Route Output](Screenshots/result_safetypath.png)

---

## 👩‍💻 Credits

Developed by **Bindu Sundarapu**   
> Passionate about using AI/ML and Python to solve real-world problems.

---


