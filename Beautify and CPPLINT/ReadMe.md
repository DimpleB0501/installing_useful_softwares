# Installing atom-beautify (used for alignment and formatting of the code)
  - Open Atom
  - Click on **Packages**
  - Goto **Settings View**
  - Click on **Install packages/Themes**
  - Type **uncrustify** in the search bar.
  - Select **atom-beautify**
  - You will see **Settings** goto **C++** select **Beautify on Save**. Add **uncrustifyConfig.cfg** path to **Config path**.
  

Than follow https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce-1
Follow steps 1st

Than follow this
https://github.com/Unibeautify/docker-beautifiers
Do the docker or last step with sudo


CCPLINT
Use it by the following command
python cpplint.py src/ObjectAnalytics/intruder.h
Or 
Python cpplint.py <path>
