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
