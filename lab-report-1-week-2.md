# How to Log Into a Course-Specific Account on `ieng6`:

## Step 1: Installing Visual Studio Code

![Installing Visual Studio Code](download.png)

 - Vistual Studio Code is a free coding editor that supports any programming languages without switching editors.

  - To install VS Code, visit the website [https://code.visualstudio.com/](https://code.visualstudio.com/) and download the version of program that correctly corresponds to your operating system. When installed, the opening window will look like this.

![Opening Visual Studio Code](OpeningPage.png)


## Step 2: Remotely Connecting

![Course-specific account for CSE15L](account.png)

- In order to connect to a remote computer host, we  have to look up our course-specific account for CSE15L on the website: [https://sdacs.ucsd.edu/~icc/index.php](https://sdacs.ucsd.edu/~icc/index.php). Your course-specific account should be similar to "cs15lwi22zz", with the last 3 characters being specific to your account.

- Next, we will open a terminal in VS Code by using Ctrl or Command + `, or use the Terminal --> New Terminal menu option.

- Enter the command, ``ssh cs15lwi22zz@ieng6.ucsd.edu``, but replace the `zz` with your course-specific account.

- If this is the first time connecting to the server, a message may ask if you want to continue connecting to the remote host. Type `yes` and press enter, then enter your password. This process should look similar to picture presented below. The terminal is now connected to the remote server!

![Connecting to Server](RemoteConnecting.png)

## Step 3: Trying Some Commands

![Running Commands](Commands.png)

- Try running some commands in different ways, both on your computer and on the remote computer after logging into your ssh. Here are some useful commands to try:

```
    cd ~
    cd 
    ls -lat
    ls -a
    ls <directory>
```
- Additionally, to log out of the remote server in your terminal you can type Ctrl-D or run the command `exit`.

## Step 4: Moving Files over SSH with scp

![SCP](scp.png)

When working remotely, I am able to copy files from the local directory of my computer to a remote sever such as ieng6. In this case, I am copying the file titled WhereAmI.java. Afterwards, I used the command, ls, to show that the file can be found in my home directory. I am now able to run the java file using javac and java on my computer. 

5. Setting an SSH Key

![SSH Key](SSHkeys.png)

An SSH key is an access credential that is used when accessing the SSH protocol. Ultimately, SSH keys provides the user to securely access a remote computer without the need for a password. As seen within the picture, I was able to run the program, ssh-keygen, which allowed me to create the files, public key in the server, and private key on the client. These are stored in the .ssh directory of the computer, allowing me to use these files in place of my password. At this point, I have successfully created these files but I am still unable to ssh without entering my password. 

![SSH Login](SSHLogin.png)

6. Optimizing Remote Running






