📦 Snapdrop
Fast, local, and secure media sharing via QR code.

📌 Overview
Snapdrop is a lightweight Flask-based web application that allows users to upload and view media (images and videos) locally from any device on the same network. It generates a QR code pointing to the server's local IP, making file access on mobile devices seamless and instant — no installation or internet required.

🌟 Key Features
🚀 Instant Flask Web Server
Launches locally on port 5000 and auto-starts in background
📷 Image & Video Upload Support
Accepts .jpg, .png, .gif, .webp, .mp4, .mov, .avi, .webm
🖼️ Auto-Gallery Display
Uploaded media is shown in a clean, responsive gallery view
📱 QR Code Access
Instantly generate a scannable QR linking to your local server
🖥️ Cross-Device Compatibility
Access the app from any device on the same Wi-Fi using the QR or IP

🛠️ Technology Stack
Python 3 (Flask) – Backend framework for routing and file handling
HTML + Jinja2 – Templating engine for gallery rendering
Pillow (PIL) – Image validation
qrcode – QR code generation
Socket – Local IP detection
Waitress – Production-ready WSGI server
Subprocess / Pythonw – Background execution without console window

⚙️ How It Works
Startup
main.py detects your local IP and generates a QR code linking to http://<your-ip>:5000.
Server Launch
run.py starts the Flask server in the background using waitress.
Upload Flow
Open the QR code on your phone or device
Upload images/videos directly from the browser
Files are stored in static/uploads/ and immediately rendered in a grid

🧠 What I Learned
Building a media-sharing utility with Flask and local networking
Handling file uploads and MIME-type filtering securely
Implementing platform-independent QR code access using local IP
Running Python servers in background without console interference
Designing practical tools for local use without relying on the cloud

🧪 Future Enhancements
🔐 PIN-code access or simple authentication
🧼 Auto-cleanup or storage limit for uploaded media
📤 Drag-and-drop interface for better UX
🌐 Optional remote access with tunneling (ngrok / cloudflare tunnel)
📸 Auto-thumbnail preview for videos

Snapdrop makes it effortless to share files locally without cables, accounts, or apps — just scan and go.
