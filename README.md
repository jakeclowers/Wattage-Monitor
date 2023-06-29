# Wattage-Monitor
Wattage Calculator / Monitor 
Wattage Monitor
This project aims to create a wattage monitor that collects wattage information from AMD CPUs and NVIDIA graphics cards and sends the data to Google Cloud using Google Sheets API. This repository provides the necessary code and instructions to set up the monitor.

Prerequisites
Before setting up the wattage monitor, ensure that you have the following:

An AMD CPU and/or NVIDIA graphics card(s) installed in your system.

Python 3.x installed on your system.

Access to a Google account.

**Installation
**
To install and set up the wattage monitor, follow these steps:

Clone this repository to your local machine:

**Copy code**

git clone https://github.com/jakeclowers/Wattage-Monitor.git

Install the required dependencies by running the following command in the project's root directory:

**Copy code**

pip install -r requirements.txt
Set up Google Sheets API:

Go to the Google Developers Console.
Create a new project or select an existing project.
Enable the Google Sheets API for your project.
Create credentials for the API and download the JSON file.
Rename the JSON file to credentials.json and place it in the project's gspread directory.

Configure the Google Sheets API endpoint:

Open the config.py file in the project's root directory.
Replace the SHEET_ID variable with the ID of your Google Sheets document. The ID can be found in the URL of the document.
Save the changes.
Usage
To run the wattage monitor, execute the following command in the project's root directory:

Copy code
python monitor.py
The monitor will start collecting wattage information from the AMD CPU and NVIDIA graphics card(s) in your system. It will periodically send the data to the Google Sheets API endpoint.

Troubleshooting
If you encounter any issues, ensure that you have correctly set up the Google Sheets API credentials and provided the correct SHEET_ID in the config.py file.
Make sure you have a stable internet connection for the monitor to successfully send data to the Google Sheets API endpoint.
Refer to the project's documentation or open an issue in the repository if you need further assistance.
Contributing
Contributions to this project are welcome. Feel free to open pull requests or submit issues with any suggestions, bug fixes, or improvements. This is a beginner project of mine, to monitor my energy usage, and see the effiency of the new 40 series and 7000 series gpus and cpus.

License
This project is licensed under the MIT License. Feel free to modify and distribute the code for personal or commercial use.

Acknowledgments
This project was inspired by the need for monitoring wattage information from AMD CPUs and NVIDIA graphics cards.
