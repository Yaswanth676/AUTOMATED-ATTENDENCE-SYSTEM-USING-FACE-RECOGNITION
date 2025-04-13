Here's a comprehensive `README.md` file tailored for your GitHub repository based on the provided attendance system code:

---

# 📸 Face Recognition Attendance System

This is a **Python-based Face Recognition Attendance System** that automatically marks student attendance using real-time face recognition, estimates distance from the camera to ensure optimal positioning, and sends email alerts to absent students.

---

## ✨ Features

- ✅ Real-time face recognition using webcam
- 🧠 Face distance estimation with on-screen feedback (Good Distance / Move Back / Move Closer)
- 📝 Automatic attendance marking and Excel file management
- 📧 Sends email alerts to absent students
- ⚠️ Detects and warns if multiple faces are present in the frame
- 💡 Displays current attendance status on demand

---

## 🛠 Requirements

Install the following Python packages before running the system:

```bash
pip install opencv-python face_recognition numpy pandas openpyxl
```

Make sure you have:

- Python 3.6+
- A webcam
- Valid email credentials for sending absent alerts

---

## 📂 Project Structure

```
attendance_system/
├── attendance.xlsx           # Excel file to store attendance
├── images/                   # Folder containing student face images
├── attendance_system.py      # Main source code
├── README.md                 # You're here!
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/attendance-system.git
cd attendance-system
```

### 2. Add Student Images

- Save face images of each student in the `images/` folder.
- Use clear, front-facing images.

### 3. Update the Code

Inside `attendance_system.py`:

- Replace `"USER_NAME"` with actual student names.
- Replace `"IMAGE_PATH"` with the image paths (e.g., `"images/john.jpg"`).
- Replace `"USERMAIL@gmail.com"` with student emails.
- Set your email and app password (Gmail recommended for easier SMTP):

```python
sender_email = "youremail@gmail.com"
sender_password = "your-app-password"
```

### 4. Run the Program

```bash
python attendance_system.py
```

---

## 🖥 Controls

- Press **`d`** to display current attendance status in the console.
- Press **`q`** to quit and send absent alerts via email.

---

## 📊 Attendance Output

- Attendance is logged in `attendance.xlsx`.
- Each entry includes:
  - Student Name
  - Date
  - Status (Present/Absent)
  - Time of recognition

---

## 🔐 Email Alert Notes

- You must enable **less secure app access** or **App Passwords** in your Gmail account to use SMTP.
- Consider using an environment variable or `.env` file for email credentials in production.

---

## 📸 Sample Screenshot

> _You can add a screenshot of the app in action here._

---

## 🧑‍💻 Author

- Developed by [Your Name]
- Feel free to contribute or raise issues!

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more info.

