
# Installing software in Ubuntu 18.04 (command line)
- Install google chrome
`wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`<br/>
`sudo dpkg -i google-chrome-stable_current_amd64.deb`<br/>
`google-chrome`<br/>

- Install Kazam (online video recording software)
`sudo apt-get update`
`sudo apt-get install kazam`

- Install Atom (editor)
`sudo add-apt-repository ppa:webupd8team/atom`
`sudo apt-get update`
`sudo apt-get install atom`
To remove atom `sudo apt remove --purge atom`

- Install Shotcut (video editor)
`sudo apt install libsdl2-dev`
`sudo add-apt-repository ppa:haraldhv/shotcut`
`sudo apt-get update && sudo apt-get upgrade`
`sudo apt install shotcut`

