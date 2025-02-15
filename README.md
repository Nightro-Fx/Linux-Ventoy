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
- Also, Download the Windows 10/11 ISO: https://www.microsoft.com/en-us/software-download/
- Be sure to save these files into your Downloads folder for easier access
- Now, Insert your USB drive into the USB port

# Setting up Ventoy on your USB
- Extract the `tar.gz` and open the extracted folder
- Look for a file named `VentoyGUI.x86_64` and run it
- It will open a GUI once you have entered your password
- Click on the **OPTIONS** button on the top-left of the windows
- Hover over "Partition Style", then select **MBR** for a Legacy system or **GPT** for a UEFI system.
- If your unsure about your system type, then run: `ls /sys/firmware/efi`. If the fire exists then your running a UEFI system
- Once you have selected your Partition Style, Just press "Install".
- Once installed, You may close the windows a copy your Windows iso  file to the usb drive. 
- Please do not extract the iso file, Leave it in the USB drive as is.
