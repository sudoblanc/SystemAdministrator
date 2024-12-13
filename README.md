# SystemAdministrator
# System Administration Script

A Python-based command-line tool for performing common system administration tasks, including user management, directory organization, and system health monitoring. 

---

## Features

1. **User Management**  
   - Create single or batch users from a CSV file.  
   - Update user passwords.  
   - Delete users.  
   - Validate usernames to ensure proper format (no spaces).

2. **Directory Organization**  
   - Organize files within a directory by file type.

3. **System Health Monitoring**  
   - Monitor CPU and memory usage at 1-minute intervals.
   - Check disk space usage and alert if thresholds are exceeded.

4. **Centralized Logging**  
   - Logs errors and system health information with timestamps.  
   - Logs are stored in `error_log.log` and `system_health.log`.

---

## Requirements

- **Python Version**: Python 3.6 or later
- **Dependencies**:  
  Install required packages using:
  ```bash
  pip install psutil


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




         

      
      




  
