# Naukri_Resume_Auto_Update
🔄 Naukri.com Auto Resume Uploader using Selenium This Python script automates the process of logging in to your Naukri.com account and uploading your updated resume. It's useful for keeping your profile active and appearing more frequently in recruiter searches.
🚀 Features
Auto login to Naukri.com
Navigates to your profile page
Uploads the updated resume PDF
Closes browser after completion
🧰 Requirements
Python 3.7 or higher
Google Chrome browser
ChromeDriver (matching your Chrome version)
🛠️ Installation Guide
1. ✅ Install Python
Download and install Python from the official site:
https://www.python.org/downloads/

During installation:

✅ Check the box that says Add Python to PATH
✅ OR manually set the Environment Variable after installation:
Right-click on This PC > Properties
Click Advanced system settings
Click Environment Variables
Under System Variables, find and edit Path
Add the path to your Python installation (e.g., C:\Python311\ and C:\Python311\Scripts\)
2. ✅ Install Required Python Packages
Open terminal / command prompt and run:

pip install selenium
3. ✅ Download ChromeDriver
Check your Chrome version by visiting: chrome://settings/help

Download matching ChromeDriver from:
https://sites.google.com/chromium.org/driver/

Or downlode it from Google apis (update this URL according to you chrome version and win 32 or 64 ) https://storage.googleapis.com/chrome-for-testing-public/135.0.7049.85/win64/chromedriver-win64.zip

Extract the downloaded file and do the following:

📁 Folder Structure Setup
Create a folder C:\WebDriver
Place your downloaded chromedriver.exe file inside this folder.

Create another folder C:\NaukriResume
Place your latest resume in PDF format inside this folder with the exact filename:
resume_updated.pdf

📝 Setup Script Configuration
Open the script and update these variables with your actual data:

EMAIL = "your_email@example.com"
PASSWORD = "yourNaukriPassword"
CHROMEDRIVER_PATH = "C:\\WebDriver\\chromedriver.exe"
RESUME_FILE_PATH = "C:\\NaukriResume\\resume_updated.pdf"
Make sure:

CHROMEDRIVER_PATH points to the correct chromedriver.exe location.
RESUME_FILE_PATH points to your latest resume PDF.
▶️ How to Run
Simply open command prompt in the script directory and run:

python naukri_resume_auto_update.py
It will:

Open Naukri.com
Login with your credentials
Upload your resume
Close the browser
❗ Notes
Your credentials are stored in plain text — use with caution.
Make sure your Naukri account is active and working.
Resume file must be a valid .pdf or .docx.
💡 Pro Tips
Schedule this script weekly using Windows Task Scheduler to keep your profile fresh!
Avoid running it too frequently to prevent account restrictions.
⏰ Automate with Task Scheduler or PowerShell
To keep your Naukri profile always fresh, you can automate this script to run daily or weekly using:

✅ Windows Task Scheduler
Open Task Scheduler on Windows
Click Create Basic Task
Give it a name like Naukri Resume Auto Update
Set the trigger (e.g., Daily or Weekly)
Action: Select Start a Program
Browse to:
C:\Path\To\python.exe
and in Add arguments, write:
C:\Path\To\naukri_resume_auto_update.py
Click Finish — you're done! ✅
✅ PowerShell Script (Optional)
You can also create a .ps1 script:

Start-Process "python.exe" "C:\Path\To\naukri_resume_auto_update.py"
Then schedule this .ps1 file in Task Scheduler.

💡 Pro Tip: Run the script during early morning hours to increase visibility when recruiters start their day!
