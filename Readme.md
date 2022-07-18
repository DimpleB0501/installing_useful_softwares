# Docker
- User https://hub.docker.com/ to search
- File name should be Captial Dockerfile
- sudo docker build .-t myalpineimg:2020 (imagename:tag) 
- sudo docker run myaplineimg:2020

# Embedded video playing in PDF in presentation mode in UBUNTU

### Install okular pdf viewer
```
sudo apt-get install okular --fix-missing
```

### Install VLC player

`sudo apt update`<br/>
`sudo apt install snap -y`<br/>
`sudo snap install vlc`<br/>

### Change the backend of Phonon
```
sudo apt install phonon-backend-vlc
```
On newer versions of Ubuntu, the crucial package is `phonon4qt5-backend-vlc`.<br/>
Run your pdf file in presentation mode in okular and you will be able to play embedded videos. 

# Git
`sudo apt install git`<br/>


# Installing software in Ubuntu 18.04 (command line)
- Install google chrome<br/>
`wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`<br/>
`sudo dpkg -i google-chrome-stable_current_amd64.deb`<br/>
`google-chrome`<br/>

- Install Kazam (online video recording software)<br/>
`sudo apt-get update`<br/>
`sudo apt-get install kazam`<br/>

- Install Atom (editor)<br/>
`sudo add-apt-repository ppa:webupd8team/atom`<br/>
`sudo apt-get update`<br/>
`sudo apt-get install atom`<br/>
To remove atom `sudo apt remove --purge atom`<br/>

- Install Shotcut (video editor)<br/>
`sudo apt install libsdl2-dev`<br/>
`sudo add-apt-repository ppa:haraldhv/shotcut`<br/>
`sudo apt-get update && sudo apt-get upgrade`<br/>
`sudo apt install shotcut`<br/>

- Foxit (pdf viewer)<br/>
`cd /tmp`<br/>
`wget http://cdn01.foxitsoftware.com/pub/foxit/reader/desktop/linux/2.x/2.4/en_us/FoxitReader2.4.1.0609_Server_x64_enu_Setup.run.tar.gz`<br/>
`tar -xvf FoxitReader*.tar.gz`<br/>
`sudo ./FoxitReader.enu.setup.2.4.1.0609\(r08f07f8\).x64.run`<br/>
Thank click on `next`<br/>

- VLC player
`sudo apt update`<br/>
`sudo apt install snap -y`<br/>
`sudo snap install vlc`<br/>

# Installing nvidia drivers for ubuntu 16
https://ubuntuhandbook.org/index.php/2019/04/nvidia-430-09-gtx-1650-support/
