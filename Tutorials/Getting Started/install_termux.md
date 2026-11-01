# How To Install Termux

## Method 1: F-Droid (Recommended)
1. Install F-Droid from [this link](https://f-droid.org/en/)
2. Once you have installed it, search Termux and find this:
![1000095488](https://github.com/user-attachments/assets/a310968a-7a6b-48eb-a782-ed3f3475d20a)
3. Download and install Termux. If Google Play Protect gives a warning, press "Install anyway (unsafe)".

## Method 2: GitHub
1. Go to [Termux's official GitHub repository](https://github.com/termux/termux-app)
2. Find the Releases tab
![1000095490](https://github.com/user-attachments/assets/d98bd747-496a-4392-b5af-94280d3702b9)
3. Install the APK of Termux depending on your arch. If you're unsure, install the universal build.

## Method 3: GitHub Actions (Build Workflows)
The [GitHub Actions page](https://github.com/termux/termux-app/actions) hosts builds that are created automatically from the latest source code. it include changes that haven't been released yet, so they can be newer than the official releases, but they are debug builds and may contain bugs.

1. Sign in to your [GitHub account](https://github.com/login) because you can't install as an anonymous user.  
2. Open the [Build workflow runs from the `master` branch](https://github.com/termux/termux-app/actions/workflows/debug_build.yml?query=branch%3Amaster+event%3Apush).
3. Open the most recent run with a blue checkmark.
4. Scroll down to the **Artifacts** section at the bottom of the run summary.
5. Download the ZIP that matches your device:
   * Android 7 or newer: the name must contain `apt-android-7`.
   * Android 5 or 6: the name must contain `apt-android-5`.
   * Pick the APK for your architecture: `arm64-v8a` for most phones, `armeabi-v7a` for older 32-bit devices, or `x86_64`/`x86` for emulators. If you're unsure, choose `universal`, which works everywhere but is much larger.
6. Extract the ZIP and install the APK inside it.

> **Note:** These builds are compatible with the APKs from [GitHub Releases](#method-2-github), but not with F-Droid or Google Play builds. If you're switching from F-Droid or Google Play, uninstall Termux and any Termux plugins first, which deletes everything stored in Termux (back up your files if needed). GitHub builds are also `debuggable` and signed with a [public test key](https://github.com/termux/termux-app/blob/master/app/testkey_untrusted.jks), so only install them from the official Termux repository. GitHub deletes old artifacts after a while (90 days by default), so older runs may no longer have downloads.

## Method 4: Google Play Store
Although it is NOT recommended to install Termux from Google Play Store, you can install it from [here](https://play.google.com/store/apps/details?id=com.termux).
