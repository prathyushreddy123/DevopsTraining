# Initial Installations Needed to start

Local linux Enviroment is needed to start working on the projects. Below is the better approach that I can suggest for Window Users and Mac have the Linux OS where Mac users can directly work on the linux terminal.

Follow the below steps to install and setup WSL on Windows 10 and above.
1. Obey the [document](https://learn.microsoft.com/en-us/windows/wsl/basic-commands#install) to install WSL. In brief type "wsl --install" in windows prompt to get the linux terminal
2. Provide your username and password.
3. Update the packages (sudo apt update && sudo apt upgrade).

## Visual Studio Code (Not Visual Studio) Installation for IDE.
Follow [guide](https://visualstudio.microsoft.com/downloads/) to install the same.

## AWS Account creation.
Login into **aws.amazon.com** and follow the steps to register with an email ID.

## Github Account and ssh key creation for seamless login
Login into **github.com** and create the account with email ID.
Go to the WSL linux terminal and create the ssh key pair with command `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`

The above command will generate a public and private key pair. By default, these files are saved in ~/.ssh directory with the names id_rsa (private key) and id_rsa.pub (public key).

Copy the key and Log in to your GitHub account and navigate to Settings > SSH and GPG keys. Click on "New SSH key" and paste the copied public key into the "Key" field. 

Test the connection from WSL Linux to github 

