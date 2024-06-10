
## LIGHT VERSION FROM ZIKYU 7 TVBOX PWN

Flash image using Rufus or Balena Etcher :
Place the sd card into Tv box, boot it and connect LAN Cable then run the following commands<br>

If you are login using user . use "sudo " command in <br>
If you are login using root , do not use <br>

## CLEAN INSTALL

<br>

```sh
sudo apt update
sudo apt install git -y
git clone https://github.com/zikyu8/tvboxpwn
sudo mkdir /boot/firmware/
cd tvboxpwn
sudo cp -r PPPwn /boot/firmware/
cd /boot/firmware/PPPwn
sudo chmod 777 *
sudo bash install.sh
```

## UPDATE / REINSTALL
[for 6th command ,  dont forget to change zikyu to your username armbian ] , in ex your username is tvbox1 , change this command to ( cd/home/tvbox1 ]
<br>

```sh
sudo rm -f -r tvboxpwn
sudo rm -f -r PI-Pwn
sudo systemctl stop pipwn
cd /boot/firmware/
sudo rm -f -r PPPwn
cd /home/zikyu
git clone https://github.com/zikyu8/tvboxpwn
cd tvboxpwn
sudo cp -r PPPwn /boot/firmware/
cd /boot/firmware/PPPwn
sudo chmod 777 *
bash install.sh
```
<br>

During the install process you will be asked to set some options.<br>
