
---

# 📖 Plagiarism Checker

A **Flutter-based plagiarism detection application** that identifies literal text plagiarism using the **KMP (Knuth-Morris-Pratt)** algorithm.
The backend is powered by a **Flask (Python) API**, enabling fast text analysis and seamless integration with the app.
The app comes with **Firebase authentication**, **dark/light mode support**, and a **modern clean UI**.

<img width="1919" height="939" alt="image" src="https://github.com/user-attachments/assets/4f48edd3-323f-4972-9688-b65e489cb7c8" />
<img width="1907" height="800" alt="image" src="https://github.com/user-attachments/assets/ad6b7918-5379-4526-b06d-8b3b2ac24487" />


---

## 🚀 Features

| Category                 | Features                                                                                                                                                                                                                |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Plagiarism Detection** | - Uses **KMP algorithm** for efficient text matching.<br>- Highlights plagiarized content within text.<br>- Displays plagiarism **percentage** and matched sources.                                                     |
| **Authentication**       | - Secure **Sign-In / Sign-Up** using **Firebase Authentication**.<br>- Persistent login sessions.                                                                                                                       |
| **UI/UX Enhancements**   | - Welcome Screen.<br>- Onboarding Screen (shown only once).<br>- Splash Screen before app launch.<br>- Clean Input UI for text submission.<br>- Results with plagiarism highlights.<br>- **Dark & Light mode** support. |
| **Backend API (Flask)**  | - REST endpoints for plagiarism detection.<br>- Processes text against stored reference materials.<br>- Returns JSON response with plagiarism details.                                                                  |

---

## 🛠️ Tech Stack

| Layer                        | Technologies                                                                                                      |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **Frontend (Flutter)**       | Flutter & Dart<br>GetX (state management & navigation)<br>Firebase Authentication<br>Dynamic theming (Light/Dark) |
| **Backend (Flask - Python)** | Flask (REST API)<br>Text preprocessing & string matching<br>KMP Algorithm for plagiarism detection                |

---

## 📱 App Flow

```
Splash Screen → Onboarding Screen (first launch only) →
Welcome Screen → Sign-In / Sign-Up (Firebase) →
Home Screen (enter text) → Analysis Screen (results with highlights & %)
```

---

## 📂 Project Structure

```text
PlagiarismChecker/
│── lib/
│   ├── main.dart
│   ├── screens/
│   │   ├── splash_screen.dart
│   │   ├── onboarding_screen.dart
│   │   ├── welcome_screen.dart
│   │   ├── signin_screen.dart
│   │   ├── signup_screen.dart
│   │   ├── home_screen.dart
│   │   └── result_screen.dart
│   ├── controllers/
│   ├── models/
│   └── widgets/
│
│── backend/
│   ├── server.py       # Flask server
│   ├── reference_texts # Folder containing source documents
│   └── utils.py        # KMP algorithm & preprocessing
│
│── README.md
│── pubspec.yaml
│── requirements.txt
```

---

## ⚡ Getting Started

### ✅ Prerequisites

* Flutter SDK installed
* Firebase project configured
* Python 3.8+
* Flask installed (`pip install flask`)

### 🔹 Backend Setup

```bash
cd backend
pip install -r requirements.txt
python server.py
```

### 🔹 Flutter Setup

```bash
cd plagiarism_checker
flutter pub get
flutter run
```

---

## 📌 Future Improvements

* Support for **semantic plagiarism detection** (not just literal).
* Integration with **external document databases**.
* Support for **PDF/DOCX uploads**.

---

