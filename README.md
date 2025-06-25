# StegoVault-Project
# 🕵️‍♂️ StegoVault – Secure Message Vault

**StegoVault** is a full-stack web application that allows users to **hide (encode)** and **reveal (decode)** secret messages within PNG images using **LSB steganography**. It offers a simple, user-friendly interface to securely transmit confidential information, protected with a password. Built entirely with **JavaScript**, it includes a custom dark mode, voice playback, and instant download functionality.

---

## 🚀 Features

- 🔐 Hide messages inside PNG images securely
- 🔓 Decode hidden messages using a password
- 🌓 Toggle between Light and Dark themes
- 🔊 Speak the decoded message using Text-to-Speech
- 📥 Download the stego image instantly after encoding
- 🛡️ Password protection using simple steganographic rules

---

## 🛠️ Tech Stack

### 💻 Frontend
- **HTML** – Page structure
- **CSS** – Responsive and modern UI styling
- **JavaScript (Vanilla)** – Interactivity and API communication
- **Web APIs** – `fetch`, `FormData`, `SpeechSynthesis`, `DOM`

### 🌐 Backend
- **Node.js** – JavaScript runtime environment
- **Express.js** – REST API server framework
- **Multer** – File upload handling (PNG images)
- **PNG.js** – Read and manipulate PNG pixels
- **CORS** – Enable secure frontend-backend communication
- **fs** – Handle file system operations

---

## 📁 Project Structure

stegovault/
│
├── backend/
│ ├── server.js # Express server + encode/decode logic
│ ├── package.json # Node.js dependencies
│
├── frontend/
│ ├── index.html # UI layout
│ ├── style.css # Theme and styling
│ └── script.js # JS logic for encode/decode + API calls
│
└── README.md

**💡 How It Works**
**▶️ Encoding (Hiding a Message)**
--Upload a .png image

--Enter your secret message and password

--The message is embedded into the least significant bits (LSBs) of the red channel of each pixel

--A 00000000 binary marker is appended to signify the end of the message

--The result is a stego image that can be downloaded instantly

**🔍 Decoding (Revealing a Message)**
--Upload the stego PNG image

--Enter the password used during encoding

--The backend reads pixel LSBs, reconstructs the binary message, and validates the password

--The final message is displayed and can be spoken aloud

**🧪 Example Use Cases**
--Securely transmit short passwords or access codes via image

--Educational demonstration of LSB-based steganography

--Personal or academic cryptography projects

**🔒 Security Notes**
--Only PNG images are supported (to ensure pixel accuracy)

--Password and message are concatenated as password::message before encoding

--For added security, AES encryption can be integrated (future enhancement)







