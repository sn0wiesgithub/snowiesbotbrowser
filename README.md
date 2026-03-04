#some apt packages needed:

sudo apt install python3-pyqt5 
sudo apt install python3-pyqt5-webengine
sudo apt install python3-pip
sudo apt install cryptogaphy
#or 
sudo apt install python3-cryptography
#also 
#if not work
pip install cryptography --break-system-packages

#also if still no pyqtwebengine:
#or windows pc
pip install pyqt5 pyqtwebengine cryptography pyqt --break-system-packages

#install pyinstaller:
sudo apt install pyinstaller
#or
sudo apt install python3-pyinstaller 
#or
pip install pyinstaller --break-system-packages

#when build with pyinstaller dont forget add the icon 
#for windows 7/10/11:

pyinstaller --onefile --add-data "snowybot.js;." --noconsole --icon=images.ico snowybrowser.py

#for linux :
pyinstaller --onefile --add-data "snowybot.js:." --noconsole --icon=images.ico snowybrowser.py

#then in the dists folder there's your app
# note also in some distros pyqt5 can just be pyqt

#run also with
python3 snoybrowser.py 
