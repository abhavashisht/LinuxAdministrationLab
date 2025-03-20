# Experiment 5  

## Question  
1. **Implement `ps`, `top`, and `kill` commands with their options.**  
2. **Installing, updating, and removing software using the `apt-get` command.**  

## Description  

In this experiment, we will:  
- Use the `ps`, `top`, and `kill` commands to **monitor and manage processes**.  
- Use `apt-get` to **install, update, and remove software** in Debian-based Linux distributions.  

## Screenshot  
<img width="920" alt="Screenshot 2025-03-20 at 8 30 09 PM" src="https://github.com/user-attachments/assets/2f626cf8-fb32-4b21-9926-3c56ef98cb94" />
<img width="740" alt="Screenshot 2025-03-20 at 8 30 37 PM" src="https://github.com/user-attachments/assets/24680679-da71-415c-9e2a-cbcd73369a86" />
<img width="636" alt="Screenshot 2025-03-20 at 8 31 28 PM" src="https://github.com/user-attachments/assets/7402274c-641a-47cd-899a-5c896ae3a0aa" />
<img width="1084" alt="Screenshot 2025-03-20 at 8 32 00 PM" src="https://github.com/user-attachments/assets/417321f5-7d9e-476b-881a-f554b76dbe1d" />
<img width="1119" alt="Screenshot 2025-03-20 at 8 32 42 PM" src="https://github.com/user-attachments/assets/5d24f1f9-82dc-4cd8-809d-143148835fae" />
<img width="1470" alt="Screenshot 2025-03-20 at 8 35 51 PM" src="https://github.com/user-attachments/assets/2826004a-0a1d-4404-a0a4-a3e1deec957c" />
<img width="1470" alt="Screenshot 2025-03-20 at 8 37 46 PM" src="https://github.com/user-attachments/assets/42129086-f152-4d7d-9410-fc4606b816ca" />
<img width="918" alt="Screenshot 2025-03-20 at 8 38 36 PM" src="https://github.com/user-attachments/assets/b0d59b32-6391-42b6-8262-abd03d942a21" />

## Commands Used  

### **1️⃣ Process Management Commands**  

```bash
# List all currently running processes
ps aux  

# Display a tree view of running processes
ps -ejH  

# Show processes of a specific user (replace username accordingly)
ps -u username  

# Display real-time system processes with CPU & memory usage
top  

# Show only processes of a specific user in top (replace username)
top -u username  

# Kill a process using its PID (replace <PID> with actual process ID)
kill <PID>  

# Kill all instances of a program by name (e.g., kill all Firefox processes)
killall firefox  

# Kill a process forcefully (SIGKILL)
kill -9 <PID>  

# Update package lists before installing new software
sudo apt-get update  

# Upgrade all installed packages to the latest versions
sudo apt-get upgrade  

# Install a specific software package (replace package_name accordingly)
sudo apt-get install package_name  

# Remove a package but keep its configuration files
sudo apt-get remove package_name  

# Remove a package and its configuration files completely
sudo apt-get purge package_name  

# Auto-remove unnecessary dependencies after package removal
sudo apt-get autoremove  

# Clear local package cache to free up space
sudo apt-get clean  
# Auto-remove unnecessary dependencies after package removal
sudo apt-get autoremove  

# Clear local package cache to free up space
sudo apt-get clean  







