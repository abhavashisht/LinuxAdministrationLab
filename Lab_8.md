# **Experiment 8: Shell Scripting and Redirection in Linux**  

## **Question**  
1. **Write a shell script to print system information.**  
2. **Write a shell script to perform basic mathematical calculations.**  
3. **Use redirection operators to store the output of commands.**  

## **Description**  
In this experiment, we will:  
- **Write a shell script** to display system information such as OS details, CPU usage, and memory status.  
- **Create a shell script** to perform basic mathematical calculations (addition, subtraction, multiplication, division).  
- **Use redirection operators** (`>`, `>>`) to store command output in files.  

## **Screenshot**  
<img width="734" alt="Screenshot 2025-03-20 at 9 01 46 PM" src="https://github.com/user-attachments/assets/e0408552-a026-401e-bc67-cbacdb7fadb9" />
<img width="728" alt="Screenshot 2025-03-20 at 9 00 54 PM" src="https://github.com/user-attachments/assets/2b851079-4d0e-4c35-bd01-eb29c927c8cc" />
<img width="1470" alt="Screenshot 2025-03-20 at 9 04 37 PM" src="https://github.com/user-attachments/assets/d09e5d5e-60ee-406b-95fb-06ffb0b9ff89" />
<img width="740" alt="Screenshot 2025-03-20 at 9 03 03 PM" src="https://github.com/user-attachments/assets/5292b8f1-0bd0-43cb-9355-3617de239b9d" />

## **Commands & Scripts Used**  

### **1️⃣ Shell Script to Print System Information**  
**Create a script file named `sys_info.sh`**  

```bash
#!/bin/bash

echo "===== System Information ====="
echo "Hostname: $(hostname)"
echo "Operating System: $(uname -o)"
echo "Kernel Version: $(uname -r)"
echo "CPU Information: $(lscpu | grep 'Model name')"
echo "Memory Usage: "
free -h

echo "Disk Usage: "
df -h

chmod +x sys_info.sh
./sys_info.sh

** Create a script file named math_calc.sh
#!/bin/bash

echo "Enter first number: "
read num1
echo "Enter second number: "
read num2

echo "Select operation: "
echo "1. Addition"
echo "2. Subtraction"
echo "3. Multiplication"
echo "4. Division"
read choice

case $choice in
    1) result=$((num1 + num2))
       echo "Result: $result" ;;
    2) result=$((num1 - num2))
       echo "Result: $result" ;;
    3) result=$((num1 * num2))
       echo "Result: $result" ;;
    4) if [ $num2 -ne 0 ]; then
           result=$((num1 / num2))
           echo "Result: $result"
       else
           echo "Error: Division by zero!"
       fi ;;
    *) echo "Invalid choice!" ;;
esac

chmod +x math_calc.sh
./math_calc.sh

./sys_info.sh > system_info.txt
cat system_info.txt

./math_calc.sh >> calculations.txt
cat calculations.txt



