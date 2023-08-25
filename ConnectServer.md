# Server

## How to connect to Server

### Probably Some pre-steps I don't know with HawkID registration

Move on only if you have configured VPN, HawkID successfully and make sure the internet is all good.

### Connect Server through FastX
Download and install FastX2 client through this [link](to be filled, probably host the installation package somewhere safe).

Open FastX2

Click on plus sign
```
Here is a sample Configuration. Remember to replace the variables with your specific value.

Name: itf08-YOURNAME
Host: itf08.psychiatry.uiowa.edu
Port: 22
User: HAWKID-MAYBE?
Sci: bin/sci

NO Forward Agent Connections
```

Double-click the configuration, a prompt should pop-up asking for password of `HAWKID`.

After fill password and connect successfully, click up-right `plus` sign to add a gnome session.

After gnome session launched, swipe up to unlock and type in the  password of `HAWKID`.

### Connect Server through SSH

Open terminal on workstation.

Copy below command to terminal
```
ssh YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu
```

Type in  password of `HAWKID`

Hit `enter` key

## File manipulation with remote server
### How to copy file from remote server to local workstation
```
scp YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu:/path/to/remote/file /path/to/local/destination
```

### How to sync folder from remote server to local workstation
```
rsync -avz -e ssh /path/to/source/ YOUR_HAWK_ID@itf08.psychiatry.uiowa.edu:/path/to/destination/
```
## How to use Rclone to mount server folder

## Concepts
### SSH
SSH = Secure Shell
- Used to connect to remote server
- After connection, interact with the server through Command Line


