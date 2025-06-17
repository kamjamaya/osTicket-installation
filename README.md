![image_alt](https://github.com/kamjamaya/osTicket-installation/blob/5b8ffcda83d48fdd945b6a29e80c08605440e04f/osTicket-logo.png)

# osTicket Installation

This tutorial outlines the prerequisites and installation of the open source ticketing system, osTicket.

# Environments and Technologies Used

- Microsoft Azure Virtual Machines
- Remote Desktop
- Internet Information Services (IIS)

# Operating Systems Used

- Windows 10 Pro V2 x64

# Deployment and Configuration Steps

Download the osTicket Installation Files: [osTicket file download](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD) 

Once they are downloaded, drag the files to the desktop.

![image_alt](https://github.com/kamjamaya/osTicket-installation/blob/437a1d68c482f357fb48168e6e13930a60b4f1fe/osTicketInstall%201.png)

Right-click on the folder and select “Extract All."

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/eb66329e27d0dfcce673b0539bc8730ff4fb533f/osTicketInstall%202.png)

Click "Extract."

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/45fcdbd4743c68e7fbdb7e93a10ae4104b62d3b4/osTicketInstall%203.png)

After the files are extracted there should be 2 shortcuts of the installation files on your home screen, you can put the original shortcut in the Recycle Bin. We only want to work with the files that have been extracted or unzipped.

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/90131791f795e4a13c79270818b4fc82899ba34f/osTicketInstall%204.png)

Next we need to enable IIS in Windows with CGI. To do that go to the start menu in the left bottom corner and type control panel in the search bar and open it. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/6db11e2a65885eeee125cc0e3ce566b610e1a954/osTicketInstall%205.png)

Under Programs, click “Uninstall a program.” 
On the left hand side, click on “Turn Windows features on or off.”

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/26804d297fbfe0a8c27e0d17b26c458f4247649f/osTicketInstall%206.png)

Check the Internet Information Service box. Click on the "+" to expand it.
Check the box of World Wide Web Services, expand it, check the box of Application Development Features, and then you will see the CGI box that we are looking for. Make sure to check that box as well. Click "OK' after that. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/dd7bbaf6f40cd1acd165f9e2db8193e501a1fcbb/osTicketInstall%207.png) 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/e041a11c893c98b0c664f4c2b4b1a32994b8917e/osTicketInstall%208.png)

Next we are going to install PHP manager for IIS.
First go to the osTicket Installation files we unzipped on the desktop.
Double-click on "PHPManagerForIIS_V1.5.0"

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%209.png)

Click next and I agree to finish installing it.

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2010.png)

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2011.png)

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2012.png)

Within that same folder we are going to install the rewrite module.
Click on “rewrite_amd64_en-US” to install it. Click Install on the pop-up menu that comes up for it. Click finish to finish the installation. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2013.png)

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2014.png)

Open another window of file explorer. You can do this by right-clicking on the folder icon located on the taskbar. On the left side right click where it says “Windows (C:)
Click on “New” and then “folder”.

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/c159e6a98999f3130ecbd6da2702be461c808bd3/osTicketInstall%2015.png)

Name the New Folder “PHP” and then in the osTicket Installation files folder right click the PHP folder, “php-7.3.8-nts-Win32-VC15-x86”. Click extract all. You should see this screen that asks you to select a destination and extract files. Browse to the PHP folder we made or you can simply type it in, in the space provided. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/215ec5b0aacdf5bd5fad74c9ff280569dce70495/osTicket.png)

Click "Extract."
Now, when you go to the PHP file in the Windows C: drive you should see all of the php files from the osTicket Installation in that folder.
Next, we are going to install C++ redistributable by double clicking on the VC_redist.x86 file from the osTicket Installation file folder. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/fa27f8e1d780d3762b27b5e8e7cf9b823dccbf8b/osTicketInstall%2017.png)

Check the I agree box and click install

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicketInstall%2018.png)

Once it is done installing you will see this screen.

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicketInstall%2019.png)

 Next, we are going to install MYSQL 5.5.62. It is in the file folder for osTicket Installation files. 

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicket%20Install%2020.png)

Double-click it and this screen should pop up for it. Click next.

![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicketInstall%2020.png)

 Accept the terms and click "Next."

 ![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicketInstall%2021.png)

  Click "Typical" and then "Next." 

   ![image_url](https://github.com/kamjamaya/osTicket-installation/blob/57c5e55c0e84ea2bc36cfe1fb58c3b6a2ac48b36/osTicketInstall%2022.png)
