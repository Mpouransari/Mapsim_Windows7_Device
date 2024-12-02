# Mapsim_Windows7_Device
Windows 7

---


This `README.md` file provides a comprehensive, step-by-step guide in English for generating an SSH key, adding it to GitHub, and testing the SSH connection. It also includes common troubleshooting tips to help users resolve potential issues.

---

## Step 0      

*After Download [Zip File](https://github.com/Mpouransari/Mapsim_Windows7_Device.git) 

-Run [Mapsim_installer_windows7.py]

- You need install [Python 3.8.10](https://www.python.org/ftp/python/3.8.10/python-3.8.10.exe) For Windows 7

-And install in CMD:
          
          pip install python-dotenv


# Steps to Generate and Use an SSH Key for GitHub Access (Windows)

This guide will walk you through the steps to generate a new SSH key and add it to your GitHub account, allowing you to use GitHub repositories without entering a password each time.

## Prerequisites

1. **Git Bash**: Ensure that you have **Git Bash** installed on your system. If not, you can download and install it from the following link:
   
   - [Download Git V2.47.1 for Windows](https://github.com/git-for-windows/git/releases/download/v2.47.1.windows.1/Git-2.47.1-32-bit.exe)
     
   - OR
     
   - [Download Git Last Version For Windows](https://git-scm.com/)
     

3. **GitHub Account**: You should have an active GitHub account. If you don't have one, you can create it [here](https://github.com/join).

---

## Step 1: Install Git Bash

1. Download and install **Git Bash** from the link above.
2. After installation, open **Git Bash**.

---

## Step 2: Generate a New SSH Key

1. Open **Git Bash**.

2. In the Git Bash terminal, enter the following command to generate a new SSH key:

   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

Replace "your_email@example.com" with the email address associated with your GitHub account.

This command will create a new SSH key using the RSA algorithm and a key size of 4096 bits.

When prompted to "Enter a file in which to save the key," press Enter to accept the default file location. By default, this is:

          /c/Users/YourUsername/.ssh/id_rsa

* If you have already created an SSH key, you can either overwrite it or save it with a different name.
Next, you will be asked to enter a passphrase (optional). Enter a passphrase for additional security, or press Enter to leave it empty (this is optional, but recommended for better security).

---

## Step 3: View and Copy the SSH Public Key in Git Bash


Once the key is generated, view your new SSH public key with the following command:

          cat ~/.ssh/id_rsa.pub

This will display the SSH public key in the terminal. It will look similar to the following:
ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEArjRPYcA1g7HJtt1My... (long key)
Highlight and copy the entire public key text. You can use your mouse or the keyboard shortcut Ctrl + Shift + C to copy it.

if not copy in Git Bash :

 - Copy & Past in ** CMD ** :

          type %USERPROFILE%\.ssh\id_rsa.pub


---

##Step 4: Test Your SSH Connection to GitHub

To verify that everything is set up correctly, run the following command in Git Bash:

-           ssh -T git@github.com

If everything is working correctly, you should see a message like this:

           "Hi your_username! You've successfully authenticated, but GitHub does not provide shell access.
            This means your SSH key is correctly added and you can now interact with GitHub repositories without needing to enter a password each time."

successful . . . 🔥

---

##Step 5: 

Send Public Key to Us With [Telegram](https://t.me/Tarantula_support_bot) 

And Wait for Activation .

---



