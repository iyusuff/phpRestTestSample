# phpRestTest

<a name="Requirements" />
# Requirements

* [GIT Version Control client](https://git-scm.com/)
* [php]
* [Composer]

<a name="running-locally" />
# Running locally

git clone https://github.com/iyusuff/phpRestTestSample.git

cd to /phpRestTestSample

composer install

phpunit testrest.php


<a name="Tips" />
#One time setup - SSH for PHPStorm to work with GIT

The PhpStorm git Integration man page does mention:
ssh keys are generated outside PhpStorm. You can follow the instructions from http://inchoo.net/tools/how-to-generate-ssh-keys-for-git-authorization/ (see below Head1 or 2) or look for other guidelines.
Store the ssh keys in the home_directory \.ssh\ folder. The location of the home directory is defined through environmental variables:
$HOME for Unix-like operating systems.
%userprofile% for the Microsoft Windows operating system.
Make sure, the keys are stored in files with correct names:
id_rsa for the private key.
id_rsa.pub for the public key.

Head 1: Windows
Just follow these 5 steps:

Go to this address, and download msysgit, after the download install it with default settings
Open Git Bash that you just installed (Start->All Programs->Git->Git Bash)
Type in the following: ssh-keygen -t rsa (when prompted, enter password, key name can stay the same)
Open file your_home_directory/.ssh/id_rsa.pub with your favorite text editor, and copy contents to your Git repository’s keys field (GitHub, beanstalk, or any other repository provider), under your account.
Be sure that you don’t copy any whitespace while copying public key’s content (id_rsa.pub)
Note: your_home_directory is either C:\Users\your_username (on Windows Vista / 7), or C:\Documents and Settings\your_username (on Windows XP)

Head 2: Mac
Follow these 5 steps:

Start the terminal
Navigate to your home directory by typing: cd ~/
Execute the following command: ssh-keygen -t rsa (when prompted, enter password, key name can stay the same)
open file you’ve just created ~/.ssh/id_rsa.pub with your favorite text editor, and copy contents to your Git repository’s keys field (GitHub, beanstalk, or any other repository provider), under your account.
Be sure that you don’t copy any whitespace while copying public key’s content (id_rsa.pub)