<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <h1 align="center">
        <img src="https://github.com/Nightro-Fx/Linux-Ventoy/blob/main/Title.png" width="600" alt="Logo"/> 
    </h1>
  
  <p align="center">
  <a href="https://discord.gg/kNHaaFsGZ2">
    <img src="https://github.com/Nightro-Fx/Performance-FastFlags/blob/main/img/Discord_Join.png" alt="Join Now" width="150">
  </a>
</p>
<p align="center">
  <a href="https://www.youtube.com/@Nightro-Fx">
    <img src="https://github.com/Nightro-Fx/Performance-FastFlags/blob/main/img/Subscribe_Hover.png" alt="Sub Now" width="130">
  </a>
</p>
</body>
</html>

# Getting Started
First we need to download all the file needed
- Download the latest verion of Ventoy: https://sourceforge.net/projects/ventoy/files/v1.1.02/
- Generate an unattend file for debloating: https://schneegans.de/windows/unattend-generator/
- Also, Download the Windows 10/11 ISO: https://www.microsoft.com/en-us/software-download/
- Be sure to save these files into your Downloads folder for easier access
- Now, Insert your USB drive into the USB port

# Setting Up Ventoy on Your USB

1. Extract the `.tar.gz` file and open the extracted folder.
2. Look for a file named `VentoyGUI.x86_64` and run it.
3. Enter your password when prompted; this will open the GUI.
4. Click on the **OPTIONS** button in the top-left corner of the window.
5. Hover over **Partition Style**, then select **MBR** for a Legacy system or **GPT** for a UEFI system.
6. If you're unsure about your system type, run the following command in the terminal: `ls /sys/firmware/efi`
- If the command returns output, you are running a **UEFI** system.  
- If the directory does not exist, you are running a **Legacy** system.  
7. Once you have selected the partition style, click **Install**.
8. After installation, close the window and copy your Windows ISO file to the USB drive.
9. **Do not extract the ISO file**—leave it as is in the USB drive.  


# Setting Up VentoyPlugson (Optional)
We will use this to set up the `autounattend.xml` file in Ventoy.

1. Navigate to the directory where the `VentoyGUI.x86_64` file is located.
2. In the same directory, you will find `VentoyPlugson.sh`. We will execute this script from the terminal.
3. Right-click on an empty space and select "Open in Terminal."
4. In the terminal, run: `lsblk` and identify your USB drive. It should be something like **sda1**.
5. Run: `sudo bash VentoyPlugson.sh /dev/sda1`, and note the IP address from the output.
6. The IP address should be something like `http://127.0.0.1:24681/`.
7. Paste your **XML** file into your USB drive.
8. Open the website from the previous step and navigate to **AutoInstall Plugin**.
9. Configure your `ventoy.json` file to recognize your autoinstall file.

