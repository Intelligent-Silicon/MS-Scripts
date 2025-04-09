# MS-Scripts & Utilities.
 Links to useful MS Scripts and Utility apps for configuring Windows PC's and Servers.
 
 
 ### Dev Box setup
 
 A link to Microsoft's Github account with a script for setting up a standard Dev Box aka a Developer's PC.
 The script removes apps which are not usually needed in the course of writing software. 
 Useful for configuring virtual PC's that are used for automated testing purposes.  
 
 https://github.com/microsoft/windows-dev-box-setup-scripts
 
 
 ### VenToy
 
"Ventoy is an open source tool to create bootable USB drive for ISO/WIM/IMG/VHD(x)/EFI files.
With ventoy, you don't need to format the disk over and over, you just need to copy the ISO/WIM/IMG/VHD(x)/EFI files to the USB drive and boot them directly.
You can copy many files at a time and ventoy will give you a boot menu to select them."

To install Windows 11 with a local account, its neccesary to remove any network connection to the internet when you install windows. During the installation process, press Shift and F10, some laptops may require you to press Shift, Fn and F10. This opens up a command line window, where you next need to type
oobe\bypassnro
then press enter. Windows will reboot and then not get stuck in a loop looking for a wifi or ethernet cable connection that connects to the internet which in turn forces you to have a Microsoft Live.com or Outlook.com account and other cloud services. This also means you can create a local user account that is only stored on the computer in question, which is how windows has worked for years.
 
 https://www.ventoy.net
 
 
 ### Power Toys
 
 Yes Microsoft Power Toys still exist.
 
 https://github.com/microsoft/PowerToys
 
 
 ### AutoUnattend
 
 A website to create and configure an AutoUnattend.xml which is searched for and used to automatically install Windows. This can prevent installation of software which can be removed using the MS Dev Box scripts. Your own scripts can be added to the AutoUnattend.xml file to further configure the Windows box during and immediately after installation. This is useful for those who spend a bit of time, adjusting windows to suit their individual preferences and way of working, including installing additional programs which support command line installations.
To use, just download and install the Windows 10/11 installation assistant, select the version of windows you want to install, select the USB stick to download and copy onto.

https://www.microsoft.com/en-us/software-download/windows11

https://www.microsoft.com/en-gb/software-download/windows10


Once completed, just copy the AutoUnattend.xml file into the root folder of the USB stick and boot up your computer with the USB stick plugged in..

To install drivers for your computer, create a folder on the USB stick, calling it Drivers, download them from the internet and extract them into their own subfolder. The Windows Installation software will automatically search and detect the drivers on the USB stick and install them during the installation process. *Note* Not all drivers can be extracted into their own subfolder, but have to be installed from a command line prompt or manually using its setup wizard window aka installation window. Where the driver installation software will accept a command line prompt, this can be included in a script file, and then just call the script file from the AutoUnattend.xml file.

 
 https://schneegans.de/windows/unattend-generator/
 
 
 ### God Mode
 
 Create a folder on your desktop and call it/rename it:
 ```
 God Mode.{ED7BA470-8E54-465E-825C-99712043E01C}.
 ```
 The icon will change from the default folder icon to the control panel icon, where it lists all the control panel options in one big list. 
 If you dont like it, just delete the folder.
 
 As more of the control panel options are moved to the new Windows Setting window (gear icon with a blue centre), you can still access the control panel, by searching for "Control Panel" in the taskbar search box, open it, then right mouse click on the control panel icon now visible on the taskbar, and choose Pin to Taskbar to pin it to the taskbar. Some control panel icons will take you back to the Windows Setting window, as Microsofts move them to the new part of the system.
 
 
 Additional utilities will be added over time if I find them useful for myself.
 
