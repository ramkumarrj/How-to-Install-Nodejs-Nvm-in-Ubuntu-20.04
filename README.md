# How to Install Nodejs in Ubuntu-20.04

#### Refresh your local package index first by typing
````
sudo apt update
````

#### Then install Node.js:
````
sudo apt install nodejs
````

#### Check that the install was successful by querying node for its version number:
````
node -v
````

#### If the package in the repositories suits your needs, this is all you need to do to get set up with Node.js. In most cases, you’ll also want to also install npm, the Node.js package manager. You can do this by installing the npm package with apt:
````
sudo apt install npm
````

# Install NVM for changing Node Version

#### Before piping the command through to bash, it is always a good idea to audit the script to make sure it isn’t doing anything you don’t agree with. You can do that by removing the | bash segment at the end of the curl command:
````
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh
````

#### Take a look and make sure you are comfortable with the changes it is making. When you are satisfied, run the command again with | bash appended at the end. The URL you use will change depending on the latest version of nvm, but as of right now, the script can be downloaded and executed by typing:
````
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
````

#### This will install the nvm script to your user account. To use it, you must first source your .bashrc file:
````
source ~/.bashrc
````

#### If you are using the interactive terminal to test installing Node.js with nvm, you will need to source your the ~/.bash_profile file instead. Use the following command to do so:
````
source ~/.bash_profile
````

#### Now, you can ask NVM which versions of Node are available:
````
nvm list-remote
````
