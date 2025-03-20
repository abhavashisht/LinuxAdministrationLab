# Experiment 3:  

## Question  
Use `Vim` and `nano` to edit the **editing_final_lab.txt** file.  
- Use the **lab_file** shell variable.  
- Enter **visual mode** in Vim.  
- Remove the **last seven characters** from the **first column** on the **first line**.  
- Preserve only the **first four characters** of the **first column**.  

## Description  

In this experiment, we will:  
1. **Open & Edit the File**  
   - Use `nano` and `vim` to edit the `editing_final_lab.txt` file.  
   - Use the `$lab_file` shell variable for file handling.  
2. **Modify Text in Vim**  
   - Enter **visual mode** to modify the first line.  
   - Remove the last **seven characters** from the first column.  
   - Keep only the **first four characters**.  

## Screenshot  
<img width="1470" alt="Screenshot 2025-03-20 at 7 56 55 PM" src="https://github.com/user-attachments/assets/6456e343-0649-4aea-9e0f-d5f8e5d9d8ca" />
<img width="494" alt="Screenshot 2025-03-20 at 8 01 42 PM" src="https://github.com/user-attachments/assets/7ef80470-63a6-4c0f-8d91-95cd72416bd4" />

## Commands Used  

```bash
# 1. Create the lab_file shell variable
lab_file="editing_final_lab.txt"

# 2. Create and open the file using nano
nano $lab_file

# 3. Create and open the file using Vim
vim $lab_file

# 4. Enter visual mode in Vim
# Press `Esc` and type:
v

# 5. Navigate to the first line
gg

# 6. Select the last 7 characters of the first column
0 → l (move right) → v (visual mode) → 7x (delete)

# 7. Preserve only the first four characters
# Move the cursor to the 5th character and delete everything after it
0 → 4l → d$

# 8. Save and exit Vim
Esc → :wq → Enter
