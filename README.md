# Real-Time Face Recognition Attendance System

## Overview
This project implements an automated attendance system using real-time face recognition. The system detects and recognizes faces from a live video feed, logs attendance in real time, and stores the data in an Excel sheet.

## Features
- Real-time face detection and recognition.
- Attendance logging with name and status (e.g., Present/Absent).
- Efficient storage of attendance data in an Excel sheet using the `openpyxl` library.
- High accuracy for known individuals using robust facial encodings.

## Technologies Used
- **Python**: Programming language.
- **OpenCV**: For video capture and image processing.
- **face_recognition**: For facial detection and recognition.
- **dlib**: For underlying facial encoding and landmark detection.
- **openpyxl**: For managing attendance data in Excel files.
- **Webcam/Camera**: For capturing live video streams.

## Requirements
### Software
- Python 3.7+
- Libraries:
  ```bash
  pip install opencv-python face_recognition dlib openpyxl
  ```

### Hardware
- A computer with at least 4GB RAM.
- Webcam for video capture.

## Setup and Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/real-time-face-recognition.git
   cd real-time-face-recognition
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add known face images to the `images/` folder. Ensure each image is named as the person's name (e.g., `John.jpg`).

4. Run the application:
   ```bash
   python attendance.py
   ```

5. The application will:
   - Capture video from the webcam.
   - Recognize known faces and mark their attendance.
   - Save the attendance to `output.xlsx` in the project directory.

## Project Structure
```plaintext
real-time-face-recognition/
├── images/                # Folder for storing known face images
├── attendance.py          # Main application script
├── requirements.txt       # Required Python libraries
├── output.xlsx            # Output Excel sheet (generated after running)
└── README.md              # Project documentation
```

## Example Output
- **Console:**
  ```plaintext
  Detected: John
  Detected: Alice
  Attendance logged successfully.
  ```

- **Excel File (output.xlsx):**
  | Name  | Attendance |
  |-------|------------|
  | John  | Present    |
  | Alice | Present    |

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and open a pull request.

