## Test Case 2 — File Permission Configuration


**Scenario:** A web server requires a properly configured `index.html` file with specific ownership and access permissions.

### Tasks

1. Navigate to your home directory and create a file named `index.html`.
2. Add any HTML text content to the file.
3. Check the file's current default permissions.
4. Grant full permissions (read, write, execute) to all users on the file.
5. Change the file owner and group to `www-data`.
6. Change the file permissions to `755`.
7. Display the final permissions and ownership to verify the configuration.

### Expected Outcome

- File `index.html` exists in the home directory with content.
- After step 4, permissions show `rwxrwxrwx`.
- After step 5, owner and group both show `www-data`.
- Final `ls -l` output shows:
  ```
  -rwxr-xr-x 1 www-data www-data ... index.html
  ```

---
