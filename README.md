# configuration

…or create a new repository on the command line

echo "# configuration" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/halobraindotcom/configuration.git

git push -u origin main


…or push an existing repository from the command line

git remote add origin https://github.com/halobraindotcom/configuration.git

git branch -M main

git push -u origin main




You can use GitHub Desktop on Ubuntu, but it’s not officially supported by GitHub — only Windows and macOS are officially supported. The Linux version comes from a community-maintained fork (shiftkey/desktop) that works very similarly and is widely used on Ubuntu.

 Install via APT Repository (Recommended)
This sets up a repo so updates come through Ubuntu’s package system.
Open a terminal.


Add the GPG key and repo:


wget -qO - https://mirror.mwt.me/shiftkey-desktop/gpgkey | gpg --dearmor | sudo tee /etc/apt/keyrings/mwt-desktop.gpg > /dev/null

sudo sh -c 'echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/mwt-desktop.gpg] https://mirror.mwt.me/shiftkey-desktop/deb/ any main" > /etc/apt/sources.list.d/mwt-desktop.list'


sudo apt update

sudo apt install github-desktop
