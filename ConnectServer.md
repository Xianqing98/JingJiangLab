# Server Tutorial
Move on only if you have configured VPN, HawkID successfully and make sure the internet is all good.

University/Department server should be accessed with school Wifi or VPN connected

## Connect to argon 

### Through SSH

Open terminal on workstation.

Copy below command to terminal
```
ssh HawkID@argon.hpc.uiowa.edu
```
Type in  password of `HawkID`


## Connect to psychiatry department server

### Through SSH

Open terminal on workstation.

Copy below command to terminal
```
ssh YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu
```

Type in  password of `HAWKID`


### Through FastX
Download and install FastX2 client through this [link](to be filled, probably host the installation package somewhere safe).

Open FastX2

Click on plus sign
```
Here is a sample Configuration. Remember to replace the variables with your specific value.

Name: itf08-YOURNAME
Host: itf08.psychiatry.uiowa.edu
Port: 22
User: HawkID
Sci: bin/sci

NO Forward Agent Connections
```

Double-click the configuration, a prompt should pop-up asking for password of `HAWKID`.

After fill password and connect successfully, click up-right `plus` sign to add a gnome session.

After gnome session launched, swipe up to unlock and type in the  password of `HAWKID`.


## File manipulation with remote server
### How to copy file from remote server to local workstation
```
scp YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu:/path/to/remote/file /path/to/local/destination
```

### How to sync folder from remote server to local workstation
```
rsync -avz -e ssh /path/to/source/ YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu:/path/to/destination/
```
## Use Rclone to configure drives (Google/OneDrive)

To set up and use rclone to access Google Drive and OneDrive through the terminal, follow these steps:

1. **Install rclone:**
   If you haven't already, download and install rclone from the official website: https://rclone.org/downloads/

2. **Configure rclone:**
   Open your terminal and run the following command to configure rclone for Google Drive:
   ```
   rclone config
   ```
   Follow the prompts to set up a new remote connection for Google Drive. Provide your Google Drive credentials and choose a name for the remote connection. See https://rclone.org/drive/. (Note that to choose yes when asked if config a Team/Shared Drive)

   Repeat the same process to configure rclone for OneDrive. See https://rclone.org/onedrive/.

   




## Concepts
### SSH
SSH = Secure Shell
- Used to connect to remote server
- After connection, interact with the server through Command Line


