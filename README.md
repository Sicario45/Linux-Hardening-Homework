# Linux-Hardening-Homework
Submission guidelines answers to linux homework

Step 1
A: ls -l
B: sudo chmod user
C: ls -l /etc/gshadow
D:  sudo chmod /etc/gshadow
E:  ls -l /etc/group
F: sudo chmod /etc/group
G:  ls -l /etc/password
H:  sudo chmod /etc/password
Step 2
A: sudo adduser sam
     sudo adduser joe
     sudo adduser amy
sudo adduser sara
sudo adduser admin
B:  sudo admin group
Step 3
A:  sudo usermod -g engineers sam
sudo usermod -g engineers joe
sudo usermod -g engineers amy
sudo usermod -g engineers sara
sudo usermod -g engineers admin
B: /home/engineers
C:  sudo mkdir /home/engineers
D:  sudo chown :engineers /home/engineer





Homework Linux Systems Administrator Scenario

After running the Lynis audit these were my findings.  My warnings were that I need to update to the latest version.  The latest version is not up to date.  No password set for single mode [AUTH-9308].  The audit found one or more vulnerable packages [PKGS-7392].  Another warning is I found some disclosure in SMTP banner [mail-8810].  
After going over my suggestions.  Some programs to install to help harden the system is as follows.  Install libpam-tmpdir to set $TMP and $TMPDR for pam sessions [CUST-0280].  Install apt-list bugs to display a list critical bugs prior to each post installation [CUST-0810]. Install debian-goodies so that you can run check start after upgrades to determine which services are using old versions of libraries and need restarting [CUST-0830].
In conclusion when performing a Lynis audit “ok” does not mean the scanned target is correctly configured safe or best practice.  Where there are problems, fix the problems.  Update your systems to the latest software versions.  Create authenticated, complicated passwords.  All these practices will help harden the system.  

*** I was not able to snapshot any of my screens, so I wrote out some warnings and suggestions after running my Lynis audit.***
