# wired window manager
=====

### Welcome to the Wired

**wiredWM** is rav3ndust's personal fork of [i3](https://i3wm.org/), which is a tiling window manager for [X11](https://www.x.org/). There is also work ongoing to bring the configs over to [Sway](https://swaywm.org/), for [Wayland](https://wayland.freedesktop.org/).

![image](https://github.com/rav3ndust/wiredWM/assets/35274771/606fd9ee-4924-4d64-96f0-1de99bf3de87)

###### let's all love lain

=====

## minimal and lightweight 

![image](https://github.com/rav3ndust/wiredWM/assets/35274771/a1229952-062f-4f6e-8eb9-02e08712c081)


###### minimal desktop and keyboard-driven for quick efficiency. clickable icons are located at the right side of the status bar for common tasks - for those unfortunate occasions where you have to reach for the mouse

Easy to use and easily extensible. Takes up very little of precious system resources, and gives you a minimal but efficient keyboard-driven environment, so you can focus less on messing around with bells and whistles found on prominent desktop environments and focus more on the task at hand. It *is* a tiling window manager, and these sorts of WMs are well-loved for how efficient and extensible they can be. 

**Clickable launchers for:**

- Screenshot utility (handles via `flameshot`.)
- Network/Wi-Fi manager (handles via `nm-applet`.)
- Volume Control (handles via `volumeicon`) 
- Weather (handles via `meteo-qt`)
- Bluetooth Manager (handles via `blueman`)
  
=====

## more resources for your stuff

![image](https://github.com/rav3ndust/wiredWM/assets/35274771/1100995d-363f-45e6-8b45-a4f084d983d7)

###### browse the web and run all of your favorite applications in a minimal environment 

Just open up the **nightshade launcher** by pressing *Meta+D* - that launches a custom **dmenu** script, and you can search for and launch your applications with ease. Think of it as your miniature Start panel.

For a general list of applications, you can also press *Meta+Shift+A* and scroll through to select one. Anything that has a desktop entry will appear here. 

=====

## organize your windows with ease

![image](https://github.com/rav3ndust/wiredWM/assets/35274771/40b3d828-78a1-4af7-be99-089c440a3b57)

###### automate the organization of the windows on your screen

A bunch of floating windows can become difficult to manage in the middle of a workflow - which is another reason a tiling window manager can really come in handy. Being built on top of the much-loved **i3**, **wiredWM** allows you to easily tile or float your windows with a quick keyboard shortcut. 

=====

### custom stuff

**wiredWM** also contains: 

- custom **dmenu** and **rofi** configurations for running commands and launching applications.
- status bar giving you your connectivity stats, battery life, time and date, and handy applets for common utilities
- my own custom scripts built on top of [suckless's](https://suckless.org) **surf** browser.
- a custom **conky** config.
- custom keyboard shortcuts for some of the scripts we've built in.
- display compositing via **picom**.
- ...various other assorted things!

### handy quickstart!

Here are some of the common **keyboard shortcuts** to keep in mind when starting out: 

> Please note, the *Meta* key is also known as the *Windows* key. On Apple keyboards, the *Meta* key is the *command* key.

- **Meta+Enter**: Open a terminal.
- **Meta+D**: Open `dmenu` to run a command.
- **Meta+Shift+A**: Open Application List to launch an app. Reads from `.desktop` files.
- **Meta+Shift+D**: Open `rofi` run launcher to filter open windows and run commands.
- **Meta+Shift+Q**: Close the focused window.
- **Meta+W**: Switch to **tabbed** windowing.
- **Meta+S**: Switch to **stacked** windowing.
- **Meta+E**: Switch to **tiled** windowing.
- **Meta+Shift+R**: Restart the window manager in-place.
- **Meta+Shift+Z**: Lock your screen. We use `i3lock-fancy` for this.
- **Meta+Shift+N**: Pops out your recent notifications.
- **Meta+C**: Pops out a calendar window. We use `gsimplecal` for this.
- **Meta+Shift+E**: Log out of the session. 

> *close the world, enter the nExt* ;)

### credits 

**wiredWM** is a fork of [i3](https://github.com/i3/i3), the most glorious window manager ever made.

Some of our other major components are: 

- [rofi](https://github.com/davatorium/rofi)
- [flameshot](https://github.com/flameshot-org/flameshot)
- [nm-applet](https://github.com/pavlix/nm-applet)
- [meteo-qt](https://github.com/dglent/meteo-qt)
- [gsimplecal](https://github.com/dmedvinsky/gsimplecal)
- various components from [suckless](https://suckless.org).

### are we wayland yet?

![image](https://github.com/user-attachments/assets/7705fe4c-f98a-4919-8853-0ca072bee4ad)

As mentioned above, work has been going on to move our configs over to Sway, for Wayland. 

I want to make sure everything works as flawlessly on the Wayland version of wiredWM as it does for the x11 version, so I am keeping the two repositories separate. I have been messing around with this lately, and the Wayland version of our configs are finally becoming my daily driver.

 To that end, I will have a different repo for the Wayland version of wiredWM, so that anyone can easily grab the x11 or wayland version, whichever they prefer based on their needs.

![image](https://github.com/user-attachments/assets/5a8b7617-8e0a-42a8-ad2f-0b825f3202b6)

We're using `waybar` in place of `polybar` in our Wayland configuration.

I've put a lot of work into our `waybar` config. It has clickable modules, custom styling following our 'nightshadeNeon' color scheme, and a systray.

`xdg-desktop-portal-wlr` is also included in the installation script, for apps that use portals.

![image](https://github.com/user-attachments/assets/13aa24e2-13b7-43c9-9165-2d7738f3e42e)

We want it to be 1:1 with the x11 version, so when I'm comfy with using it as my daily driver for awhile, I'll have a new repo up and linked here! The repo you're currently in, of course, will not be going anywhere. The x11 version is going to be being kept around for a long time to come.

![image](https://github.com/user-attachments/assets/d8417ca3-10d5-4b1e-9645-956fbee058f1)

### Wayland references

Here are some great references to learn more about Wayland.

- [Wayland wikipedia entry](https://en.wikipedia.org/wiki/Wayland_(protocol)): A dive into wayland on wikipedia.
- [Wayland freedesktop site](https://wayland.freedesktop.org/): The site for Wayland with documentation, FAQ, architecture overview, repos, mailing list, and more linked in.
- [wayland-book](https://wayland-book.com): A great book from Drew Devault going over the Wayland protocol at a high-level.
- [We are wayland now!](https://wearewaylandnow.com/): A good little one-page site with a lot of resources listed, including desktops supporting wayland, screencasting tools, notification daemons, window managers, imagew viewers, and many more categories of software, so that if you are migrating to wayland, you can easily find an alternative to any x11 applications that don't (or don't plan to) support wayland.
- [sway](https://swaywm.org): Sway is what we base the wayland version of wiredWM on top of. It is a drop-in replacement for i3, and will work with your config (you'll probably have to adapt a few tools, as we have) if you're coming over from x11.
