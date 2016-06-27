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
ssh keys are generated outside PhpStorm. You can follow the instructions from http://inchoo.net/tools/how-to-generate-ssh-keys-for-git-authorization/ or look for other guidelines.
Store the ssh keys in the home_directory \.ssh\ folder. The location of the home directory is defined through environmental variables:
$HOME for Unix-like operating systems.
%userprofile% for the Microsoft Windows operating system.
Make sure, the keys are stored in files with correct names:
id_rsa for the private key.
id_rsa.pub for the public key.