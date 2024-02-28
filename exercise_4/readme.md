# Exercise

## Task:

Install PHP 7.4 on your local linux machine using the ppa:ondrej/php package repo.
Instruction:

Learn how to use the add-apt-repository command
Submit the content of /etc/apt/sources.list and the output of php -v command.

## Solution 

Steps to Install PHP 7.4 using the ppa:ondrej/php package repo

1. First run the `sudo apt-get update` to ensure you have access to the latest version of anything you want to install.

2. Next, install software-properties-common, which adds management for additional software sources:\
  `sudo apt -y install software-properties-common` The -y flag will automatically agree to the installation.

3. Next, install the repository `ppa:ondrej/php`, which will give you all your versions of PHP:\
  `sudo add-apt-repository ppa:ondrej/php` Then we do a `apt-get update` again so thaat our package manager can see newly listed packages

4. Install php with `sudo apt -y install php7.4`

5. To check the version of php run the command `php -v`