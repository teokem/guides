# INSTRUCTIONS FOR SETTING UP COMPUTERS

Instructions for setting up new macOS system at compchem; please follow in the presented order.

## Basic setup and updating

1. Power on the laptop and follow instructions for creating a user account.
   You should connect to the internet through Eduroam, using your LUCAT id.
   Remember to end your id with `@lu.se` which enables you to connect from most universities in the World.

3. When asked, create an iCloud account if you do not already have one.
   This is required to install (free) applications from Apple's App Store.
   You may be forced to enter a credit card number, but you can be remove it later.

4. Once the initial set up is finished, go to **App Store** (top-left corner)
   and install all updates showing up in the "Update" section.

5. Go to system preferences, then **Software update** and allow automatic
   upgrades of security and app updates (it is not recommended to automatically upgrade the OS version).
   
6. For laptops it's a good idea to encrypt your user data in case it gets stolen. Enable this in System Preferences -->
   Security & Privacy --> FileVault.
   
7. You may want to disable Apple's file version control which tend to take up space.
   Go to System Preferences --> General and tick (☑) _Ask to keep changes when closing documents_.

## Microsoft Office Apps

1. Go to https://www.office.com and sign in using your university email.
   You will be prompted to enter LUCAT credentials and thereafter
   taken to "Office 365" which is Microsoft's online version of office.
   Navigate to "Install Office Apps" (usually in top right corner), download and install.

2. Once installed, accept all software updates if any, and also allow
   office to automatically download updates.

## Endnote

Download the LU licensed version [here](https://program.ldc.lu.se) (look under "Alfasoft").

## Apple's Command Line Tools (CLT)

This is needed for homebrew and other development tools. Open a Terminal (`Applications/Utilities/Terminal.app`) and run
`xcode-select --install` to download and install.

## Homebrew package manager

Homebrew is a package manager for installing unix command line tools and require Apple's CLT (see above).

1. Install by running a single command line, pasted from the Homebrew frontpage, https://brew.sh

2. Search and install for packages using `brew search <package>` and `brew install <package>`

Brew can also be used to install MacOS applications such as Firefox, Skype, Spotify etc.
Some examples:

~~~ bash
brew install gcc grace coreutils gfortran
brew install --cask mactex firefox xquartz zoomus bitwarden miniforge
~~~

## Python

Python is already installed on macOS, but a convenient way of managing packages and environments is via [Conda](https://github.com/conda-forge/miniforge).
Install via `brew install --cask miniforge` as shown above.
You may now install packages like this:

~~~ bash
conda install notebook jupyter matplotlib scipy pandas
~~~

## Cloud storage and backup:

Box is a service very similar to DropBox for online storage. By default LU employees have 20 GB of free storage and the service is security approved by the university (_Dropbox is not_). If you need to expand the disk space, simply call LDC service desk (phone 29000) and give them your LUCAT id and the space you need. For laptops, it makes no sense to expand the capacity with more than the laptop disk size, i.e. typically 128 or 256 GB.

To get started with Box:

1. Install with `brew install --cask box-sync`
2. Open _Box Sync_ and login with your university email and follow the instructions.

Once installed, you will have a new folder called _Box Sync_ in your top-level user directory. All files placed here will be automatically synced to Box and _vice versa_. For example, you could install Box Sync on multiple computers and they will all be synched automatically. From the Box website you have access to version history of your files as well as the possibility to restore deleted files.

Finally, Box integrates with Microsoft's Office 360 (see above) and you can edit Word, Excell files etc. on Box directly from a web-browser without any additional software installed (for example from Linux). 

## Free access to Matlab, Maple, Comsol etc.

- Login and download using LUCAT credentials at http://program.ddg.lth.se
- Get the free Github educational pack (https://education.github.com/pack), incl. Github Copilot.
- [JetBrains](https://www.jetbrains.com/education/) professional coding IDE's are available to students and teachers.

## Printers

### General printing at LU

The large Canon printer on 2nd floor, shared between physical chemistry and theoretical chemistry, can be used only through the LU printing system PaperCut [(instructions here)](http://www.print.lu.se/english/papercut/). For every print you will need to use your access card at the printer. Employed staff pay no charge.

### Brother DCP-L3550CDW (3rd floor)

1. Make sure you're logged into Apple App Store (top left corner menu item in Finder) using your Apple ID.
   This step may be required for system preferences to automatically download the required drivers. You must also
   be on the local network (Eduroam does not work!).

2. Add manually in System Preferences->Printers->Address:

       http://130.235.1.39 (AirPrint)

## Erase and Reset

If you no longer need your mac, make sure to delete all contents by following these instructions: https://support.apple.com/en-gb/HT201065


## More help?

Once the above is complete, contact M.L. if you need additional help.
