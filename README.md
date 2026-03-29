# 📸 Face Attendance System

An automated attendance marking system that uses **facial recognition** to identify students from a single class photo and mark their attendance — no manual roll call needed.

---

## 🚀 How It Works

1. A **dataset of student face images** is collected and stored
2. When a **class photo is clicked**, the system scans all faces in the image
3. Each face is matched against the student dataset using facial recognition
4. Attendance is **automatically marked** as Present or Absent
5. Results are exported to a structured **Excel sheet**

---

## ✨ Features

- 📷 Single photo → full class attendance in seconds
- 🧠 Facial recognition using deep learning
- 📊 Exports attendance to Excel with student ID, name & status
- ✅ Handles multiple faces in one image
- 🎨 Color-coded Excel output (green = Present, red = Absent)
- 📁 Organized dataset management per student

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| face_recognition | Face detection & matching |
| OpenCV | Image processing |
| openpyxl | Excel report generation |
| Google Colab | Development environment |
| Google Drive | Dataset storage |

---

## 📁 Project Structure

```
CLASS-ATTENDANCE/
│
├── FaceAttendance_final.ipynb   # Main notebook
├── requirements.txt              # Dependencies
└── README.md                     # Project documentation

Google Drive/
├── face_dataset/                 # Student face images (one folder per student)
│   ├── Student_001/
│   ├── Student_002/
│   └── ...
├── testing_data/                 # Class photos for attendance
└── FaceAttendance/               # Generated attendance Excel sheets
```

---

## ⚙️ Setup & Usage

### 1. Clone the repository
```bash
git clone https://github.com/wakeupletscode/CLASS-ATTENDANCE.git
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Prepare the dataset
- Create one folder per student inside `face_dataset/`
- Add 3–5 clear face images per student in their folder
- Folder name = Student name or ID

### 4. Run in Google Colab
- Open `FaceAttendance_final.ipynb` in Google Colab
- Mount Google Drive
- Run all cells
- Upload or point to a class photo
- Attendance Excel sheet is auto-generated 🎉

---

## 📊 Sample Output

| S.No | Student ID | Name | Attendance |
|------|-----------|------|-----------|
| 1 | STU001 | Omkar Dey | ✅ Present |
| 2 | STU002 | John Smith | ❌ Absent |
| 3 | STU003 | Priya Sharma | ✅ Present |

---

## 📦 Requirements

```
face_recognition
opencv-python
openpyxl
numpy
Pillow
```

---

## 🔮 Future Improvements

- [ ] Real-time webcam attendance
- [ ] Web dashboard for attendance history
- [ ] SMS/email notification to absent students
- [ ] Mobile app integration

---

## 👨‍💻 Author

**Omkar Dey**  
[![GitHub](https://img.shields.io/badge/GitHub-wakeupletscode-black?logo=github)](https://github.com/wakeupletscode)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
