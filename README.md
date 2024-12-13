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
