This is a tutorial for incoming 15L students. The following instruction includes logging into CSE15L account, setting up VScode, remotely connecting, and writing command.
## Log into course-specific account
1. open this link: [link](https://sdacs.ucsd.edu/~icc/index.php)
2. Type in the username you use for logging into your normal UCSD account and your student ID.
3. The word on the button under the "**Additional Account**" is your username. It starts with "**cs15lsp23**" and ends with two random characters. ![Image](Account_setting.png)

## Install Visual Studio Code
1. Use this [link](https://code.visualstudio.com/) to install and follow the instruction on this page.
(I didn't put the image of installation process since I have installed VScode on my computer a year ago. )
The following is a screenshot of an opened-VScode page. After your installation, the opened-VScode should be like this.
![image](vsCode2.png)

## Remotely connecting
1. First of all, open the terminal by clicking the "terminal" on the top of the screen. And select "New Terminal".
![image](terminal.png)

2. On the terminal, type in the following command after the bash: `ssh cs15lsp23np@ieng6.ucsd.edu`, replace the `zz` with the two characters in your own account. Then the terinal will ask for your password.
(If it is your first time for remote connection, your computer may have error message: 
`The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?`
Simply Type in yes. Since this is not my first time to conduct remoate connect, I did not show this here.)

![image](ssh.png)

3. Type in your password. Then the terminal will show the following thing:
![image](r2.png)
![image](r1.png)
This shows that our terminal is connected to a computer in CSE basement and the command we run on our own computer will at the same time run on that computer. Our computer is called client and the computer in the basement is called server. Then we will write some command

## Run some command

![image](ls-remote.png)
I typed in the command `ls` on the remote account. The command lists the content of current directory. 

![image](ls-cs.png)
I typed in the command `ls` on my own computer.  The command also lists the content of current directory on my own computer. 

![image](cd-wavelet.png)
I typed in the command `cd wavelet` on the remote account. The command moves us to the `wavelet` directory. 

![image](cd-cs.png)
I typed in the command `cd Music` on my own computer. The command moves us to the `Music` directory.

![image](pwd-remote.png)
I typed in the command `pwd` in remote control. The command prints the current directory for me, which is `/home/linux/ieng6/cs15lsp23/cs15lsp23np`.

![image](pwd-cs.png)
I typed in the command `pwd` on my computer. The command prints the current director for me, which is `/Users/michelle/Music`.

![image](command.png)
I typed in the command `ls /home/linux/ieng6/cs15lsp23/cs15lsp23np`. The username at the very end is my own username. When I type in my username after the directory, the computer lists files in my account(directory), which is perl5. 

![image](directory-cs.png)
When I exit the remote computer and type in the same command, the terminal shows `No such file or directory`. The directory I put in is the directory on the remote computer, which could not be found on our own computer; therefore, the directory does not exist on my own computer. 

![image](lat-remote.png)
I typed in the command `ls -lat` in the remote computer. The command sorts the output on the remote computer based on the time modified. 

![image](lat-cs.png)
I also typed in the command `ls -lat` on my own computer. The command sorts the output of my computer based on the time modified. 







