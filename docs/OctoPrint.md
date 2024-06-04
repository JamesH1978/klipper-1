Start by installing [OctoPi](https://github.com/guysoft/OctoPi) on the
Raspberry Pi computer. Use OctoPi v0.17.0 or later - see the
[OctoPi releases](https://github.com/guysoft/OctoPi/releases) for
release information. One should verify that OctoPi boots and that the
OctoPrint web server works. After connecting to the OctoPrint web
page, follow the prompt to upgrade OctoPrint to v1.4.2 or later.

After installing OctoPi and upgrading OctoPrint, it will be necessary
to ssh into the target machine to run a handful of system commands. If
using a Linux or MacOS desktop, then the "ssh" software should already
be installed on the desktop. There are free ssh clients available for
other desktops (eg,
[PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/)). Use the
ssh utility to connect to the Raspberry Pi (ssh pi@octopi -- password
is "raspberry") and run the following commands:

```
git clone https://github.com/Klipper3d/klipper
./klipper/scripts/install-octopi.sh
```

The above will download Klipper, install some system dependencies,
setup Klipper to run at system startup, and start the Klipper host
software. It will require an internet connection and it may take a few
minutes to complete.