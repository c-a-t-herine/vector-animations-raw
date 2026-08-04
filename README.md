# vector-animations-raw
Maya rigs, scenes, and other resources for the Vector Robot!

Sincere thanks to [Randall Maas](https://github.com/randym32) for his generous contributions to the OSKR project and to the Vector community!

~~Building new animations requires a license to Autodesk Maya 2018-2020.~~
**This repo contains updates that should allow for building new animations using Maya 2027.**

wrt the `Victor_rig_01.ma` file location. In many of the .ma files this path is set to a user specific directory
(`"/Users/selena/workspace/victor-animation//assets/rigs/Victor_rig_01.ma"`). In many cases Maya did prompt for the path each time I opened a file,
but I found going through and updating the paths with find/replace was easier than navigating to the correct rig file repeatedly. I did not commit
any of my updated paths but example files would be  `anim_explorer_driving_01.ma` and `assets...anim_explorer_01.ma`.


Once you have installed Maya, you will need to install the AnkiMenu plugin (see the installation guide below).
Once that is done, please see the [documentation](https://github.com/digital-dream-labs/vector-animations-raw/tree/main/documentation) folder for build guidelines.

Notes:
- You will likely need to grant execution permissions on scripts being run with the Anki Plugins in Maya. For example, `$chmod +x remount-fs.sh`. I did not run every
  script because I a) did not need the functionality b) did not spend time checking the behaviour would align with my expectations. In order to preview
  animations on the robot I did use the scripts `remount-fs.sh`, `bash_cmds.sh`
- I had to assume control of the robot via the webserver before running animations
- If hitting a permission denied when trying to run the animation on the robot, if you've already given all of the necessary scripts execution permissions,
  you may need to ssh directly to the robot first. `ssh -i ssh_root_key root@<robot ip>`

# AnkiMenu Installation:

## macOS:

- Install ~~Maya 2018 or 2019~~ Maya 2027

  - Open and close it

- Install git and git-lfs with [brew](https://brew.sh/):

  - `brew install git-lfs`

  - Clone this git in your home directory:

  - `cd ~`

  - `git clone https://github.com/c-a-t-herine/vector-animations-raw.git`

- ~~Install pip for python2:~~ This project is using python 3 now! Also, I use poetry envs so I didn't use pip directly

- ~~Install the Python packages:~~ See pyproject.toml

- Copy the Maya.env:
  - Update `SVN_WORKSPACE` if `vector-animations-raw is not located in your home directory
  - `cp ~/vector-animations-raw/tools/other/Maya.env ~/Library/Preferences/Autodesk/maya/2027/`

- Open Maya!

- See Maya Animation Setup (`/documentation/Maya 2027 Setup for Animation Work.md`) for further setup instructions


**I only used a mac, so Windows and Linux instructions will be out of date. See commit history if you are looking for the original instructions**