# Windows 10 Security Assessment Tool

⚠️ **Legal Disclaimer**: This tool is for **educational purposes and authorized penetration testing only**. Unauthorized use against systems you don't own is illegal. The developer assumes no liability for misuse.

## 🔍 Features
- System Information Collection
- Screenshot Capture
- Webcam Access
- Keylogging
- Geolocation Tracking
- Automated EXE Builder
- Gmail Reporting System

## 🛠️ Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/mynameismama6zaa/HackingW10.git
   cd HackingW10
Install dependencies:

bash
pip install -r requirements.txt
First Run Configuration:

The script will prompt for:

Your Gmail address

App password (enable 2FA and generate app password)

Recipient email

🖥️ Usage
Interactive Mode:
bash
python main.py
Menu Options:

Create EXE Version - Builds standalone executable

Exit

Silent Mode (for built EXE):
bash
main.exe --auto
📂 Modules Breakdown
Function	Description	Frequency
_get_network_information	Collects system/network data	Once
screen_shot	Takes random screenshots (1-10)	Every 1-14s
capture_camera	Webcam snapshot	Once
keylogger	Logs keystrokes	Continuous
get_user_location	IP geolocation	Once
📧 Email Reporting
Uses SMTP over TLS (Gmail)

Sends separate emails for each module

Attachments include:

keylogs.txt

screenshot.png

Camera captures

System info reports
