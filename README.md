# googledisk-backup
https://shouts.dev/install-google-drive-and-schedule-backup-to-gdrive-on-centos-7


sudo wget -O drive https://drive.google.com/uc?id=0B3X9GlR6EmbnMHBMVWtKaEZXdDg
Move GDrive to /usr/sbin/drive folder by entering this command:

sudo mv drive /usr/sbin/drive
Set permission:

sudo chmod 755 /usr/sbin/drive
We have installed GDrive in our server. Let’s connect to our Google Drive account. First, open browser and login to your google account. Our GDrive will be connected to this google drive account.

Run drive command to start the authentication process. You will a link like this:

https://accounts.google.com/o/oauth2/auth?client_id=123456789123-7n0vf5akeru7on...
Copy and paste the link in the browser. Accept the permission and you will get a verification code. Copy the verification and paste back into your shell:

Enter verification code: 4/9gKYAFAJ326XIP6JJHAEhs342t35LPiA5QGW0935...
We have installed Google Drive and connected to our Google Drive account.

Step 2 : Create a Backup Shell Script
We are going to create a bash script. It will compress all files and folder. Then it will upload it to Google Drive.

Go to your Google Drive and create a folder. Go to the folder. Now, look at the URL. At the end of the URL, you can see the folder’s path. Look at the screenshot to be clear:
