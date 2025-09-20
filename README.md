# 👤 Face Recognition–Based Attendance System  

A **facial recognition–based attendance management system** built with **Python**, **OpenCV**, and a **Tkinter GUI**.  
The system allows users to mark attendance simply by facing the camera, and logs details into structured CSV files.  

---

## 🛠️ Technologies Used
- Python 3.x  
- OpenCV (Open Source Computer Vision Library)  
- Tkinter (Python GUI library)  

---

## 🚀 Features
- **Image Capture** – Capture facial images linked with an ID & Name.  
- **Training** – Train the recognition model with captured images (60 per person).  
- **Real-time Recognition** – Detect and identify faces via webcam.  
- **Attendance Logging** – Automatically record Name, ID, Date, and Time in a CSV file.  
- **GUI Interface** – Simple Tkinter interface with buttons for each action.  

---

## 📂 Project Workflow

1. **Initialization**  
   - Run `train.py`.  
   - Enter `ID` and `Name` in the input fields.  

2. **Image Capture**  
   - Click **Take Images**.  
   - The camera opens and captures ~60 samples per person.  
   - Images are saved in the `TrainingImage/` folder.  
   - Details are logged in `StudentDetails/StudentDetails.csv`.  

3. **Training**  
   - Click **Train Image**.  
   - The model is trained using OpenCV and saved as `TrainingImageLabel/Trainer.yml`.  

4. **Recognition**  
   - Click **Track Image**.  
   - The camera recognizes faces and displays `ID` + `Name`.  
   - Attendance is recorded in `Attendance/` as a CSV file with Date & Time.  

---

## 📁 Folder Structure

Face-recognition–based-attendance/
├── Attendance/                  # CSV logs of attendance
├── StudentDetails/               # StudentDetails.csv with IDs & Names
├── TrainingImage/                # Captured face images
├── TrainingImageLabel/           # Trained model (Trainer.yml)
├── haarcascade_frontalface_default.xml # Haar Cascade model for face detection
├── train.py                      # Main script with Tkinter GUI
├── objectsdemo.py                 # Supporting demo script
├── setup.py                       # Setup file
└── README.md                      # Project documentation


---

## 📊 Example Attendance Log
| ID   | Name   | Date       | Time     |
|------|--------|------------|----------|
| 1    | Alice  | 2025-09-20 | 09:15:32 |
| 2    | Bob    | 2025-09-20 | 09:16:10 |

---

## 🔮 Future Improvements
- Use **deep learning models (FaceNet, dlib, or CNNs)** for higher accuracy.  
- Add **database integration** (MySQL/Postgres) for attendance instead of CSV.  
- Deploy with a **web interface** or integrate with **mobile app**.  
- Improve handling of low-light or occluded face recognition.  

---

## 📜 License
MIT © 2025 Teenu Anand Nukavarapu  
