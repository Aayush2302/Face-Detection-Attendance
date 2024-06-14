# 📸 Face Recognition Attendance System

This project implements a face recognition-based attendance system using Python, OpenCV, and the `face_recognition` library. The system captures video from a webcam, detects faces in real-time, and marks attendance by saving the recognized face names and timestamps in a CSV file.

## 📋 Table of Contents

- [📦 Installation](#installation)
- [🚀 Usage](#usage)
- [📁 Project Structure](#project-structure)
- [⚙️ Functionality](#functionality)
- [📚 Dependencies](#dependencies)
- [🙏 Acknowledgements](#acknowledgements)

## 📦 Installation

1. Clone this repository to your local machine:
    ```sh
    git clone https://github.com/yourusername/face-recognition-attendance.git
    ```
2. Navigate to the project directory:
    ```sh
    cd face-recognition-attendance
    ```
3. Install the required packages using pip:
    ```sh
    pip install opencv-python numpy face_recognition
    ```

## 🚀 Usage

1. **Prepare the Images:**
   - 📂 Create a folder named `imagesAttendance` in the project directory.
   - 🖼️ Add images of the people you want to recognize for attendance in the `imagesAttendance` folder. Ensure that the filenames of the images are the names of the people (e.g., `JohnDoe.jpg`).

2. **Run the Attendance System:**
   - ▶️ Execute the following command to start the system:
     ```sh
     python main.py
     ```

3. **View Attendance:**
   - 📄 Attendance records will be saved in a file named `Attendance.csv` in the project directory.

## 📁 Project Structure

```
face-recognition-attendance/
│
├── imagesAttendance/       # Directory to store images for recognition
│   ├── person1.jpg
│   ├── person2.jpg
│   └── ...
│
├── main.py                 # Main script to run the attendance system
├── Attendance.csv          # CSV file to save attendance records
└── README.md               # This README file
```

## ⚙️ Functionality

- **Face Encoding:** The script reads images from the `imagesAttendance` folder and computes facial encodings.
- **Real-time Face Recognition:** Captures video from the webcam, detects faces, and matches them with the known encodings.
- **Attendance Marking:** If a face is recognized, the name and the current timestamp are recorded in `Attendance.csv`.

## 📚 Dependencies

- Python 3.x
- OpenCV
- NumPy
- face_recognition

You can install the dependencies using pip:
```sh
pip install opencv-python numpy face_recognition
```

## 🙏 Acknowledgements

- [OpenCV](https://opencv.org/) for real-time computer vision.
- [face_recognition](https://github.com/ageitgey/face_recognition) library for easy face recognition in Python.

