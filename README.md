# StegoVault-Project
# 🧊 StegoVault – Ultimate Steganography Web Vault 🔐

> **"Hide your secrets in plain sight."**  
**StegoVault** is a web-based steganography tool that allows users to securely encode secret messages inside image files and decode them later — with optional password protection, speech output, and a clean, interactive interface.

---

## 📌 Table of Contents

- [🧠 About the Project](#-about-the-project)
- [💡 Key Features](#-key-features)
- [📸 How It Works](#-how-it-works)
- [🛠️ Tech Stack](#-tech-stack)
- [🚀 Getting Started](#-getting-started)
- [📂 Project Structure](#-project-structure)
- [🌐 Deployment](#-deployment)
- [📄 License](#-license)

---

## 🧠 About the Project

**StegoVault** was built as a personal learning project during my web development internship to explore both frontend and backend development concepts. It combines **image processing** and **data hiding (steganography)** to create a practical, fun, and secure way to share private messages.

It was also my attempt to merge traditional development with **AI-assisted tools** for more productivity and creativity.

---

## 💡 Key Features

- 📷 **Upload image and encode message**
- 🔓 **Decode messages from encoded images**
- 🛡️ **Password-based double security**
- 🌙 **Dark Mode / Light Mode toggle**
- 🗣️ **Text-to-Speech playback of secret messages**
- 📱 **Mobile-responsive and clean UI**

---

## 📸 How It Works

🔐 **Encoding (Hide Message):**

1. Upload an image file (`.png` / `.jpg`)
2. Enter a secret message
3. (Optional) Enter a password for protection
4. Click **Encode**
5. Download the newly generated **secret image**

🔍 **Decoding (Reveal Message):**

1. Upload the encoded image
2. Enter the password (if used)
3. Click **Decode**
4. Read or listen to the original message

📌 Uses the **LSB (Least Significant Bit)** steganography technique under the hood.

---

## 🛠️ Tech Stack

### 🌐 Frontend
- `HTML5`
- `CSS3` (with dark/light theming)
- `JavaScript`
- `Web Speech API` (for message voice playback)

### 🧠 Backend
- `Python 3`
- `Flask` – lightweight Python web framework
- `Stegano` – steganography library for encoding/decoding
- `Pillow` – for image manipulation

### 📦 Others
- `gTTS` (optional): For generating downloadable spoken messages
- `.env` and `dotenv`: For secure API or config handling
- `Git + GitHub`: Version control
- `Netlify` or `Render`: For hosting frontend/backend

---

## 🚀 Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/stegovault.git
cd stegovault
