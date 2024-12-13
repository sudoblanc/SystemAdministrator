# SysAdmin Script

This Python script automates various system administration tasks, including user management, directory organization, system health monitoring, and log monitoring. It provides a convenient way to manage users, organize files, monitor system performance, and analyze logs for critical issues.

## Features
- **User Management**:
  - Create a single user with a specified role (admin/user).
  - Create users in bulk from a CSV file.
  - Delete users.
  - Update user passwords.

- **Directory Organization**:
  - Organize files in a specified directory by their file extensions.

- **System Health Monitoring**:
  - Monitor CPU and memory usage every minute for 10 minutes and log the data.
  - Check disk space usage in a specified directory and alert if it exceeds a given threshold.

- **Log File Monitoring**:
  - Monitor a log file for critical messages and save the results in a summary file.

## Prerequisites
- Python 3.x
- `psutil` package for system monitoring (`pip install psutil`)
- `sudo` privileges (for user management and system modifications)

## Setup

### Clone the repository
If you haven’t already cloned the repository, do so using the following command:

```bash
git clone https://github.com/yourusername/sysadmin-script.git
cd sysadmin-script



## Usage
   **General Command Format**
   - python3 sys_admin.py {subcommand} [options]
   **Subcommands**
     1. User Management:
         - Create a single user:
         - Create users from CSV file:
         - Update a user's password
         - Delete a user
            python3 sys_admin.py user --create --username <username> --role <role>
     2. Directory Management:
        - Organize files in a directory:
     4. System Health Monitoring:
        - Monitor CPU and memory usage for 10 minutes:
        - Check disk space usage

## Error Handling

- Invalid Inputs are logged in error_log.log
Example error message:
   [ERROR] Invalid username format. Usernames should not contain spaces.
   [INFO] Error logged to error_log.log.




         

      
      




  
