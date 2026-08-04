## Install Maya 2027:

1. Click the Apple menu/icon and select About This Mac
2. Click the Storage tab and make sure that you have *at least 3 GB* of disk space available on your hard-drive (Macintosh HD)

3. Within Maya 2027, click *Windows → Settings/Preferences → Plug-in Manager* and uncheck “Auto load” for everything except gameFbxExporter.bundle
4. Click *Windows → Workspaces* and then select the option box next to General (or whatever workspace you use) and use that UI to set the Menu Set to Animation
5. Click File and then select the option box next to New Scene and use that UI to set the default frame rate to 30 fps
6. Click *Windows → Settings/Preferences → Preferences*, select the Time Slider category and make sure your frame rate is set to 30 fps (also check the Playback settings while in there to ensure those are correct)

## Installing Studio Library:

A new 2.21.4 version of Studio Library was released for 2027 version of Maya.

The Maya Setup page has the following instruction for installing Studio Library for Maya 2027:

```
    Download studiolibrary from http://www.studiolibrary.com/ and move the unzipped folder to ~/Library/Preferences/Autodesk/maya/scripts
```

so if you already have that, you should now:

1. Launch Maya 2018 and confirm that Studio Library works if you run "import studiolibrary; studiolibrary.main()" in the Python Script Editor



## Update Maya 2027 configuration:
3. Within Maya 2027, click Windows → Settings/Preferences → Plug-in Manager and check “Loaded” and “Auto load” for AnkiMenu.py
4. Within Maya 2027, click File → Set Project... and set the Maya project to be the /Users/<your_name>/workspace/victor-animation directory
5. Within Maya 2027, set the shared Victor pose/anim library (Victor_StudioLibrary) by:
   1. clicking the Settings Menu in upper, right-hand corner of the Studio Library window
   2. selecting Change Root Path
   3. choosing the /Users/<your_name>/workspace/victor-animation/studioLibrary/Victor_StudioLibrary folder
