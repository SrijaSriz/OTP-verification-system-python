# OTP Verification System (Python - CLI)

A secure, command-line-based OTP (One-Time Password) verification system built in Python. It simulates email-based OTP delivery, includes expiry logic, input validation, regeneration limits, and a real-time countdown timer.

---

## 🔐 Features

- ✅ Generates secure 6-digit OTPs
- ⏳ OTP expires after configurable time (default: 3 minutes)
- 🔁 Allows OTP regeneration (max 3 times)
- ⌛ Real-time countdown timer using multithreading
- 📧 Validates email format before sending OTP
- 🚫 Handles invalid input and expired OTPs gracefully
- 💬 Interactive CLI-based user experience

---


<img width="1557" height="669" alt="image" src="https://github.com/user-attachments/assets/e89ba934-348a-4be4-945f-e35c0de5bb4d" />

---

## ⚙️ How It Works

1. User enters a valid email address.
2. A 6-digit OTP is generated and "sent" to the email (simulated).
3. A 3-minute timer starts in a separate thread.
4. User must enter the correct OTP before it expires.
5. Up to 2 OTP regenerations are allowed if needed.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- (Optional) `.env` for simulating secure config

### Run the Program

```bash
python main.py

🧪 Test Scenarios
✅ Correct OTP before expiry

❌ Incorrect OTP and retry

⏳ OTP expiry handling

🔁 OTP regeneration limit

🚫 Invalid email format

🚫 Non-numeric or malformed OTPs


🔐 Note on Security
While email sending is simulated, this system is built with security in mind. No real emails are sent, and environment variables are used for future extension to SMTP-based OTP systems.

👨‍💻 Author
Developed by SRIJA MANDAVILLI
Let me know if you’d like to:
- Add a real SMTP version for email
- Include a sample `.env` file or `requirements.txt`
- Customize for GUI or web app extensions

I can generate those too!
