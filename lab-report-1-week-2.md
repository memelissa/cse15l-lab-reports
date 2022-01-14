# Lab Report 1
#### Hello! My name is Melissa Phan and in this tutorial, I will be demonstrating how to log into a course-specific account on ieng6.

1. Installing VScode

![Installing Visual Studio Code](Installing.png)

![Opening Visual Studio Code](OpeningPage.png)

 I was able to successfully download the Visual Studio Code (for Mac) from the given website. After installing the program onto my computer, I opened the program, showing the default opening page. 

2. Remotely Connecting

![Course-specific account for CSE15L](CourseSpecificAcc.png)

![Connecting to Server](RemoteConnecting.png)

In order to connect to a remote computer, I had to look up my course-specific account for CSE15L, as seen within the first picture. By doing so, we can now verify that we can connect to the SSH host by running the given command in the Terminal: ssh cs15lwi22zz@ieng6.ucsd.edu. Using the course-specific account I obtained earlier, I successfully connected my terminal to a remote host. 

3. Trying Some Commands

![Running Commands](Commands.png)

As seen within the picture, I am running a variety of commands on the remote compter after ssh-ing. For example, the cd command (change directory) is used to change the current working directory and move between different directories. In addition to this, the ls command can be utilized to list files, whereas ls ~a will display all the files including ones that are hidden.

4. Moving Files with scp

![SCP](scp.png)

When working remotely, I am able to copy files from the local directory of my computer to a remote sever such as ieng6. In this case, I am copying the file titled WhereAmI.java. Afterwards, I used the command, ls, to show that the file can be found in my home directory. I am now able to run the java file using javac and java on my computer. 

5. Setting an SSH Key

![SSH Key](SSHkeys.png)

6. Optimizing Remote Running






