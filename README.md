# 🔐 Secure Data Encryption Web App

This Streamlit-based app allows users to securely **store** and **retrieve** their data using strong encryption techniques. It simulates a personal vault where data is encrypted using the Fernet algorithm and protected with a user-defined passkey.

## ✨ Features

- 🔑 **Login System** with hardcoded credentials
- 🔐 **Fernet Encryption** for data security
- ➕ **Insert & Encrypt Data** using a secret passkey
- 🔓 **Retrieve & Decrypt Data** with passkey verification
- ⛔ **Failed attempt limit** (3 tries) for extra security
- 🔁 **Session management** using Streamlit session state
- 🧠 **All data stored in memory** (not persisted on disk)

## 🛠️ Built With

- [Python](https://www.python.org/)
- [Streamlit](https://streamlit.io/)
- [Cryptography (Fernet)](https://cryptography.io/)
- [Hashlib (SHA-256)](https://docs.python.org/3/library/hashlib.html)

## 🔧 How It Works

1. **Login** using fixed credentials (`Ekta Khatri` / `ekki123`)
2. Navigate to **Insert Data**, add a key, your message, and a secret passkey
3. Message is encrypted and stored in session memory
4. In **Retrieve Data**, enter the same key and passkey to decrypt your message
5. App locks out after 3 incorrect passkey attempts for security
