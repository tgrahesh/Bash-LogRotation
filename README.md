# Bash Log Rotation and Backup Script

This Bash script is designed to perform log rotation and backup for a hypothetical web server. It rotates logs on a regular schedule (e.g., daily or weekly), compresses old log files, and creates backups of the rotated logs to a specified backup directory. It also takes into consideration log retention policies and error handling.

## Usage

1. **Installation**: Copy the Bash script to your web server. You can use `scp` or any other method.

2. **Configuration**:
   - Edit the script to set your specific configurations, including log directories, backup directories, rotation schedule, and retention policies.
     
3. **Configuration options**:
   - **Log Directory**: Specify the directory where the web server logs are stored.
   - **Backup Directory:** Define the directory where the rotated and compressed logs will be backed up.
   - **Rotation Schedule:** Set the rotation schedule (e.g., daily, weekly).
   - **Retention Policy:** Determine how many days or weeks of logs to retain before deletion.
     
4. **Feautures**:
   - **Log Rotation**: The script rotates logs based on the specified schedule, keeping logs organized by date or week.
   - **Log Compression:** Old log files are compressed to save space.
   - **Backup:** Rotated logs are copied to the backup directory for safekeeping
   - **Retention Policy:** Logs older than the defined retention period are deleted.
   - **Error Handling:** The script includes error handling to report any issues during the log rotation and backup process.

3. **Execute the Script**:
   - Run the script to initiate log rotation and backup. You can use a command like:

   ```bash
   ./log_rotate_backup.sh
