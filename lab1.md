**CSE15L Account**\
-Visit [Link](https://sdacs.ucsd.edu/~icc/index.php) to find your course-specifc account\
-Click on the “cs15lwi23asy” button (the last three characters may vary between people), click the change password button, and after filling out the “confirm password” field, press “enter” to reset your password
![Image](changePw.png)

**VS Code**\
-Visit [Link](https://code.visualstudio.com/download) to download the version of VS Code that you need\
-After installing it, open up VS Code\
-The following screenshot represents what you should see when VS Code opens
![Image](vs.png)

**Remotely Connecting**\
-In VS Code, open up a terminal and enter: ```ssh cs15lwi23zz@ieng6.ucsd.edu``` (the zz should be replaced with letters specific to your account)\
-If you connect to a server for the first time, you’ll receive a message saying the authenticity can’t be established (**The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?** )\
-Type “yes” and press enter.\
-Finally, enter your password (you will not be able to see what you type so type carefully)
![Image](remote.png)

**Run Some Commands**\
-Try out some commands like:
* cd (change directory)
* ls (list files and folders in path)
* ls -a (list files or directories, including hidden ones)
* ls -lat (listing of all files, newest first)
* pwd (print working directory)
* mkdir (make directory)
* cp (copy)
* cat (print content)\
-To log out the server, use Ctrl-D or the command exit
![Image](commands.png)
