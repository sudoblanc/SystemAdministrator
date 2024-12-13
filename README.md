sysadmin-script
A Python script for managing system tasks such as user management, directory organization, and system health monitoring. The script provides an easy way to perform these operations from the command line.
Setup
To get started, clone the repository and navigate into the project folder:
bash
Copy code
git clone https://github.com/yourusername/sysadmin-script.git
cd sysadmin-script
Install Dependencies
You may need to install the required Python packages. Use the following command to install them:
Copy code
pip install -r requirements.txt
•	psutil: For system health monitoring
Usage
General Command Format
css
Copy code
python3 sys_admin.py {subcommand} [options]
Subcommands
1.	User Management:
o	Create a single user:
css
Copy code
python3 sys_admin.py user --create --username <username> --role <role>
o	Create users from a CSV file:
css
Copy code
python3 sys_admin.py user --create-batch --csv <path_to_csv>
o	Update a user's password:
css
Copy code
python3 sys_admin.py user --update --username <username> --password <new_password>
o	Delete a user:
css
Copy code
python3 sys_admin.py user --delete --username <username>
2.	Directory Management:
o	Organize files in a directory by file type:
bash
Copy code
python3 sys_admin.py organize --dir <directory_path>
3.	System Health Monitoring:
o	Monitor CPU and memory usage for 10 minutes:
css
Copy code
python3 sys_admin.py monitor --system
o	Check disk space usage in a specific directory:
css
Copy code
python3 sys_admin.py monitor --disk --dir <directory_path> --threshold <threshold_percent>
Error Handling
•	Invalid inputs and errors are logged in the error_log.log file.
•	Example error message:
css
Copy code
[ERROR] Invalid username format. Usernames should not contain spaces.
[INFO] Error logged to error_log.log.
License
This project is licensed under the MIT License - see the LICENSE file for details.
 
You can copy and paste this directly into your document without formatting issues.

![image](https://github.com/user-attachments/assets/f7b24d99-c821-44da-8e52-71b063359566)
