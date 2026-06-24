# 🔐 Web Crypto API Personal Vault

A lightweight, secure micro-website for storing private text information, notes, and important links. It runs directly in the browser on any device without requiring servers or databases.

## 🚀 Live Demo
👉 [Open My Vault](https://github.io)

---

## ✨ Features

* **Fully Autonomous**: The project utilizes the browser's built-in **Web Crypto API**. It does not rely on third-party servers or external encryption libraries.
* **Client-Side Processing**: Data encryption and decryption occur locally on your device (PC or smartphone). Information is stored on the hosting server in a pre-encrypted state.
* **Translation Protection**: The code includes `notranslate` and `translate="no"` attributes. This prevents browser auto-translators from corrupting the encrypted data string.
* **Responsive Interface**: A minimalist dark-themed design (Dark Mode) that renders perfectly on both mobile screens and desktop monitors.

---

## 🛠 Tech Stack

* **HTML5 / CSS3** (CSS variables, Flexbox, responsive layout).
* **Vanilla JavaScript** (pure JS without any external frameworks).
* **Web Crypto API** (**AES-GCM 256-bit** encryption, **PBKDF2** key derivation function, and SHA-256 hashing).

---

## 📖 How to Update Your Data

Whenever you need to modify your saved links or text, follow these steps:

1. Open [your website](https://github.io) (it is recommended to use an **Incognito** window to avoid browser caching).
2. Enter your password and click **"Открыть архив"** (Open Vault).
3. Edit the text in the field (add new links or remove old ones).
4. Click the green **"Сохранить изменения"** (Save Changes) button.
5. Scroll to the very bottom of the page and **copy the generated line**:
   `let ENCRYPTED_DATA = "U2FsdGVkX1...";`
6. Go to this GitHub repository, open the `index.html` file, and click the **pencil icon** to edit.
7. Replace line **№53** with your newly copied string.
8. Click the green **"Commit changes"** button to save.

---

## ⚠️ Disclaimer
The password is used as a derivation key to decrypt data directly in your browser's RAM. It is **never saved anywhere**. If you forget your password, it will be impossible to recover your encrypted text.
