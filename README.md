# Ethical_Hacking
WiFi Scanner and Password Cracker
This Python project scans available WiFi networks and attempts to crack a selected WiFi network’s password using a brute-force approach with a password dictionary.

Warning: This tool is intended for educational purposes only. Unauthorized access to networks is illegal and unethical. Only use this tool on networks you have permission to test.

Features
WiFi Scanner: Lists available WiFi networks and displays their signal strength.
Password Cracker: Attempts to brute-force a WiFi network's password using a dictionary file.
Requirements
Python 3.x
pywifi library for managing WiFi connections in Python. Install it using:
bash
Copy code
pip install pywifi
How to Use
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/WiFiScannerPasswordCracker.git
cd WiFiScannerPasswordCracker
Run the Program:

bash
Copy code
python main.py
WiFi Scan:

The program first scans for available WiFi networks and displays a list sorted by signal strength.
Each WiFi network is shown with a number, strength, and name.
Select Target WiFi:

Input the number corresponding to the WiFi network you want to target.
Confirm your selection.
Password Cracking:

The program will prompt you to provide the file path of a password dictionary.
It will then attempt to connect to the target WiFi network by trying each password in the file until successful or until it exhausts the list.
If a password is found, it will display the password.
Code Overview
The program consists of three main functions:

wifi_scan(): Scans for available WiFi networks and lists them by signal strength.
wifi_password_crack(wifi_name): Attempts to crack the WiFi password of a given network using a password dictionary.
main(): Manages the program flow, prompting the user for input and handling exceptions.
Example Usage
python
Copy code
# To run the program
python main.py
Sample Output
Program scans available WiFi networks:

scss
Copy code
Scanning WiFi, please wait...(2)
Scanning WiFi, please wait...(1)
Scanning WiFi, please wait...(0)
Scan Completed!
--------------------------------------
No.  Strength  WiFi Name
0    90        MyHomeNetwork
1    75        CafeFreeWiFi
Select a WiFi network and provide a password dictionary file:

yaml
Copy code
Please choose a target wifi: 0
The chosen target wifi is: MyHomeNetwork. Sure? (Y/N): Y
Please use filename of password dictionary used for the brute force attack: passwords.txt
If a password is found, the program outputs:

yaml
Copy code
Connection Succeeded! Password: mypassword123
Disclaimer
Use responsibly and only on networks you have permission to test. Unauthorized access to networks is illegal.

License
This project is licensed under the MIT License.

This README provides a comprehensive overview of the project, including setup instructions, usage, and an example output, as well as a clear disclaimer regarding the ethical and legal considerations.






