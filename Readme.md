
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

