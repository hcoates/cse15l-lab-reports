Lab Report 1
==========

In this lab, I installed VSCode, remotely connected to a course-specific account in ieng6, and tested out basic commands wihtin the remote connected computer using my macbook.

Table of Contents
--------------

* Installing VSCode
* Remotely Connecting
* Trying Some Commands

Installing VSCode
--------

1. Go to the [VSCode Website](https://code.visualstudio.com/) 

![](./lab1-images/VSCode1.png)

2. Donwnload the version for your specific operating system, once its downloaded VSCode should look like this

![](./lab1-images/VSCode2.png)


Remotely Connecting
------

1. Look up your course specific account using [this link.](https://sdacs.ucsd.edu/~icc/index.php)
![](./lab1-images/Remote1.png)
2. Here you will find your course specific account, it should start with cs15Lwi23
3. Click the password reset login and follow the instructions to reset your password, selecting "no" for changing the tritonlink password
4. Open up terminal on your mac
5. In your terminal type: ssh Your_Account@ieng6.ucsd.edu (replacing Your_Account with your course specific account)
6. Since its your first time remote connecting it will ask "Are you sure you want to continue connecting (yes/no/[fingerprint])?", type yes
7. Enter your password to the password prompt, no text should appear as you type your password
8. You should have something similar to this output once you've successfully connected, to logout you can run exit or ctrl + d

![](./lab1-images/Remote2.png)


Trying Commands
------

1. Once you have remotely connected you can test out some common commands
* pwd
* cd ~
* cd ..
* ls

![](./lab1-images/cmds.png)
