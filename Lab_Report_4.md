This is week 7 lab report 4. We want to use vim to change a file and then commit it to the github.

# Log in
First of all, I log into the ieng6 as usual using `ssh cs15lsp23np@ieng6.ucsd.edu`.
![image](ssh)

# Clone repository
Then, I clone my fork of repository from my github account. The command line is `git clone https://github.com/michellehuang728/lab7.git`.
As I have cloned the repository during my lab, the terminal shows the path already exists in my case.
![image](clone)

# Run test before changing
Then, I run the test using the command `bash test.sh`. The test failed.
![image](test_failure)

# change the code file using vim
Then, I change the code file using vim. I first make the current directory into `lab7` and then enter the command `vim ListExamples.java`.
The following shows on the screen:
![image](vim_before)
I enter the vim mode. 
Key pressed: `<k><k><k><k><k><k>` to move the cursor to the `index1` in the last loop of merge method, this key maeans "up".
When we reach the line that we want to modify. 
Key pressed: `<l><l><l><l>` to move the cursor to the `1`, which means right. 
Key pressed:`<x>` to delete the character you want to delete. In this case it's `1`. 
![image](delete)
Key pressed:`<i>` to enter insert mode and then enter `2`. 
![image](insert)
Key pressed:`<esc>` to exit insert mode. 
![image](esc)
Key pressed: `:wq` to exit the vim mode.
![image](wq)
![image](vim after)

# Run test after changing
Then, I run the test by `<up><up><up><up>`(because I've write this command before) to get to the command `bash test.sh`. The test pass.
![image](test_pass)

# Commit and push
Then I commit the changes to the github by enter `git commit` in terminal. The vim window popes, I enter the message `modify ListExamples.java Here may be some more content` and then when we exit vim mode and run `git log` we will the see this message. 
![image](git_commit1)
![image](git_commit2)
Then I push the changes to the git hub. The result shows that the file in the github is also changed.
![image](gitpush)
