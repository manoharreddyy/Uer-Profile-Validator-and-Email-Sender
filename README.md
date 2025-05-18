# User-Profile-Validator-and-Email-Sender
# RegexMailer 📩

**RegexMailer** is a Python script that collects user details, validates them using **Regular Expressions (Regex)**, and sends the information via **email** using SMTP.

## 📌 Features

✅ Validates user input fields using **Regex**\
📧 Sends user details via **Gmail SMTP**\
🔒 Secure authentication using **environment variables**

---

## 🚀 Installation & Setup

### 1️⃣ Prerequisites

- **Python 3.x** installed
- **Gmail SMTP access enabled**
  - Enable **Less Secure Apps** (Not recommended)
  - OR use **App Passwords** for secure authentication

### 2️⃣ Clone the Repository

```sh
git clone https://github.com/your-username/RegexMailer.git
cd RegexMailer
```

### 3️⃣ Install Dependencies

```sh
pip install smtplib email
```

### 4️⃣ Set Up Environment Variables (Recommended)

```sh
export EMAIL_USER="your-email@gmail.com"
export EMAIL_PASS="your-app-password"
```

### 5️⃣ Run the Script

```sh
python script.py
```

---

## 🔍 Regex Patterns Used

| Field     | Regex Pattern                    | Description                                   |                |                 |                                   |
| --------- | -------------------------------- | --------------------------------------------- | -------------- | --------------- | --------------------------------- |
| **Name**  | `^[A-Za-z ]+$`                   | Allows only letters and spaces                |                |                 |                                   |
| **DOB**   | \`(0[1-9]                        | [12][0-9]                                     | 3[01])-(0[1-9] | 1[0-2])-\d{4}\` | Ensures valid `DD-MM-YYYY` format |
| **Phone** | `^[6789]\d{9}$`                  | Ensures a 10-digit number starting with `6-9` |                |                 |                                   |
| **Email** | `^[a-zA-Z0-9._%+-]+@gmail\.com$` | Allows only Gmail addresses                   |                |                 |                                   |

---

## ⚠️ Security Note

- ❌ **Do NOT hardcode your Gmail password** in the script.
- ✅ Use **environment variables** or **App Passwords** for security.
- 🔒 Never expose your credentials in a public repository.

---

## 📝 License

This project is **open-source**. Feel free to modify and improve it! 😊
