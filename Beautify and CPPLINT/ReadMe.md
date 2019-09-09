# Installing atom-beautify (used for alignment and formatting of the code)
  - Open Atom
  - Click on **Packages**
  - Goto **Settings View**
  - Click on **Install packages/Themes**
  - Type **uncrustify** in the search bar.
  - Select **atom-beautify**
  - You will see **Settings** goto **C++** select **Beautify on Save**. Add **uncrustifyConfig.cfg** path to **Config path**.
  - Install uncrustify by typing `sudo apt-get install uncrustify`


CCPLINT
Use it by the following command
python cpplint.py src/ObjectAnalytics/intruder.h
Or 
Python cpplint.py <path>
