# Week 6 Lab Report
*Quincy Sewell, CSE 15L, Section A00*

## Streamlining ssh Configuration
The following is an image of my .ssh/config file contents, as displayed in the VIM editor.
![](lab-report-3-ssh-config-file.jpg)

The next image displays me logging into my CSE 15L course-specific account on ieng6 using the alias I chose (CS15L).
![](lab-report-3-ssh-facilitated-login.jpg)

The next image captures me using the alias that I defined (CS15L) to facilitate my use of scp. One can see from this image that I copied a file called "Hello.java" in the home directory of my computer to the home directory for my user on ieng6.
![](lab-report-3-scp-facilitated.jpg)

## Set Up Github Access from ieng6
In the image below, one can see that I have added two public keys to my Github account. One is for the laptop that I regularly use, and the other is for my ieng6 account.

![](lab-report-3-publickeys.jpg)

One can see where the private key is stored on my ieng6 account in the below image. In particular, the file containing the private key is called id_ed25519. Additionally, the file entitled id_ed25519.pub contains the public key.

![](lab-report-3-publicprivatekeys.jpg)

In what follows, one can observe that I made edits to index.md (located in the repository in which this file is contained), and then proceeded to use `git add` and subsequently `git commit`. Finally, I used `git push origin main` to push the changes that I made to index.md to the origin.

![](lab-report-3-gitcommandsieng6.jpg)

The commit that I made in the above image can also be viewed at the following link:
[Commit Made in Above Image](https://github.com/qsewell/cse15l-lab-reports/commit/87f973bc8719cdeb3da56d3a6e526bbabb8e74b1)
