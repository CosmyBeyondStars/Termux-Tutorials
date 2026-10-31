# Termux Basics

## Updating Packages
It is recommended to update the packages to keep Termux up-to-date. To update the packages you can run this simple command:

* `pkg update && pkg upgrade`

This will keep the packages up to date and install updates to the existing/installed packages.

## Storage Access

Termux may need access to your internal storage to do actions properly, or browse files through the app. You can run the `termux-setup-storage` command to do that.

## Enabling Package Repositories

There's many things to install in Termux, while some of them are in different repositories. By default, the main package repository is enabled. However, you can enable the other package repositories:

* `pkg install x11-repo`: This will enable the repository of X11 (X Window System) packages, where you can install desktop environments, or desktop applications.

* `pkg install root-repo`: Enable this repository only if your device is rooted. It contains the packages/applications that require root permissions.

* `pkg install tur-repo`: This package repository is unofficial, but it contains various packages/applications that are not in Termux's official packages list. ([Learn more](https://github.com/termux-user-repository/tur))

* `pkg install glibc-repo` This package repository brings up packages and libraries which are only working on Termux GNU C Library (GLIBC) environment.

## Package Mirrors
If you are tired on waiting while updating the packages (which is checking all mirrors by group), you can do this to check only one single mirror:

1. Run `termux-change-repo`
2. Press the keys in order to select "Single mirror": Down arrow, SPACE, ENTER
<img width="1080" height="416" alt="5640" src="https://github.com/user-attachments/assets/8a7f8295-c588-4e5a-a6e4-820ed91876a5" />
3. Make sure you selected "default". Then, press ENTER again.
<img width="1080" height="283" alt="5641" src="https://github.com/user-attachments/assets/00c56f92-240e-4ebd-a266-71cd9d8a2186" />

With these steps, package syncing will be shorter!




