# vector-animations-raw
Maya rigs, scenes, and other resources for the Vector Robot!

Sincere thanks to [Randall Maas](https://github.com/randym32) for his generous contributions to the OSKR project and to the Vector community!

~~Building new animations requires a license to Autodesk Maya 2018-2020.~~
**This repo contains updates that should allow for building new animations using Maya 2027.**

Once you have installed Maya, you will need to install the AnkiMenu plugin (see the installation guide below).
Once that is done, please see the [documentation](https://github.com/digital-dream-labs/vector-animations-raw/tree/main/documentation) folder for build guidelines.

# AnkiMenu Installation:

## macOS:

- Install ~~Maya 2018 or 2019~~ Maya 2027

    - Open and close it

- Install git and git-lfs with [brew](https://brew.sh/):

    - `brew install git-lfs`

    - Clone this git in your home directory:

    - `cd ~`

    - `git clone https://github.com/digital-dream-labs/vector-animations-raw.git`

- ~~Install pip for python2:~~ This project is using python 3 now! Also, I use poetry envs so I didn't use pip directly

- ~~Install the Python packages:~~ See pyproject.toml

- Copy the Maya.env:

    - `cp ~/vector-animations-raw/tools/other/Maya.env ~/Library/Preferences/Autodesk/maya/2027/`

- Open Maya!

**I only used a mac, so Windows and Linux instructions will be out of date. See commit history if you are looking for the original instructions**