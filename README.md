
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
```
### Install dependencies

```bash
pip install psutil

```




## Usage/Examples

### General Syntax:

```bash
python3 sys_admin.py {user, organize, monitor} [options]

```

### User Management
#### Create a single user:

```bash
python3 sys_admin.py user --create --username <username> --role <role>
```
- --username: Username of the user.
- --role: User role (admin or user).

#### Create users from a CSV file:

```bash
python3 sys_admin.py user --create-batch --csv <path_to_csv_file>

```
The CSV file should contain columns: username, role, and password.

#### Update a user's password:

```bash
python3 sys_admin.py user --update --username <username> --password <new_password>

```

### Directory Organization

#### Organize a directory by file type:

```bash

python3 sys_admin.py organize --dir <directory_path>

```

#### Monitor a log file for critical messages:

```bash

python3 sys_admin.py organize --log-monitor <log_file_path>

```
### System Health Monitoring


#### Monitor system health (CPU and memory usage):
```bash

python3 sys_admin.py monitor --system

```

#### Check disk space usage:

```bash

python3 sys_admin.py monitor --disk --dir <directory_path> --threshold <disk_usage_threshold>

```
- --threshold: The disk usage percentage threshold (e.g., 80).


## Error Logging

Errors during script execution are logged in error_log.log and can be used for debugging. Critical log messages detected during log monitoring will be saved in error_summary.log.

### Logging
- The script logs errors using Python's built-in logging module, which writes to error_log.log.
- System health data is logged to system_health.log.
- Critical log messages detected during monitoring are saved to error_summary.log.
