# Home Assistant Installation

## Install Termux
Most of the Home Assistant installation work will be done on the command line. The most robust UNIX console emulator for Android is Termux. To get Termux, head to [F-Droid](https://f-droid.org/en/packages/com.termux/), download it, and install it. While you're here, download and install [Termux:API](https://f-droid.org/en/packages/com.termux.api/) and [Termux:Boot](https://f-droid.org/en/packages/com.termux.boot) too - we'll need them later.

The typing experience on a tablet touch-screen isn't the most conducive to using a command line. If you have one, connecting a Bluetooth keyboard would be helpful. If not, you could try a modified on-screen keyboard like [Hacker's Keyboard](https://f-droid.org/en/packages/org.pocketworkstation.pckeyboard/). Later on, we'll connect to the tablet via SSH, so you can use your computer for configuration and file transfers.

## Install Packages
Open up the Termux app. Notice that your home directory is `/data/data/com.termux/files/home/`, and the `etc` directory (where packages will be installed) is at `/data/data/com.termux/files/usr/etc/`. This is different than a standard UNIX operating system.

The package manager in Termux is `pkg`, which is a wrapper around `apt`. You can also use the `apt` command directly, but there's usually no need to do so.

Here are the packages to install at this stage:
- `python`: Home Assistant runs in Python, so the language needs to be installed
- `nano`: for viewing and editing files
- `termux-api`: to connect with the Termux:API app that is installed on the device
- `make`: to allow Makefiles to run
- `libjpeg-turbo`: to avoid a bug in a later step due to a missing JPEG package

Install the necessary packages with these commands (confirming with `y` when requested):
```bash
pkg updates - type Y, then N, then N again
pkg upgrade
pkg install python
pkg install nano
pkg install openssh
pkg install termux-api
pkg install make 
pkg install libjpeg-turbo
pkg install binutils
```

## Install Home Assistant
The prerequisites are now in place to install the Home Assistant package from the PyPi Python package repository:
```bash
# create a virtual environment (optional, but recommended)
python -m venv hass
source hass/bin/activate
pip install --upgrade pip
pip install -I pytz
pip install PyNaCl
pip install aiohttp_cors
pip install tzdata
export CARGO_BUILD_TARGET=aarch64-linux-android
pip install homeassistant
```

The virtual environment is optional, but recommended - if you don't use one, the packages will be installed in your "base" environment. Using a virtual environment makes your installation isolated - if you want to update your version of Python or Home Assistant, you could do so in a fresh virtual environment to make sure everything is working properly without impacting your existing installation.

## Run
Everything is now in place! With your virtual environment activated, execute `hass -v`. During this first startup, keep an eye on the output for error messages, which might indicate that something has been configured incorrectly.

If the startup succeeds, head to `localhost:8123` in a browser on the tablet - the Home Assistant homepage should appear!

For more information, here is [a Medium post](https://lucacesarano.medium.com/install-home-assistant-hass-on-android-no-root-fb65b2341126) describing this process.

# Addressing Setup
Home Assistant is now accessible from other devices which are also connected to your home network. To access Home Assistant, find your tablet's network IP address (something like `http://192.168.2.xyz`) by running the `ipconfig` command in Termux, or by logging in to your router's admin console (usually at `http://192.168.2.1`) and finding your tablet in the list of devices. Then, navigate to that address from another device using port 8123: `http://192.168.2.xyz:8123`. The Home Assistant interface should load, the same way it does for `http://localhost:8123` on your tablet.



UPD:


Part of this tutorial was taken from here:
https://lucacesarano.medium.com/install-home-assistant-hass-on-android-no-root-fb65b2341126
