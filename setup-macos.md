# INSTRUCTIONS FOR SETTING UP COMPUTERS

Instructions for setting up new macOS system at teokem; please follow in the presented order.

## Basic setup and updating

1. Power on the laptop and follow instructions for creating a user account. You should connect to the internet through Eduroam, using your LUCAT id (remember to end your id with `@lu.se` which will allow you to connect from most universities in the World).

2. When asked, create an iCloud account if you do not already
   have one. This is required to install _i.e._ Apple's developer tools etc. If you are forced to enter a credet card number, you can be remove it later.

3. Once the initial setting up is finished, go to "App Store" (top-left corner)
   and install all updates showing up in the "Update" section.

4. Go to system preferences, then "Software update" and allow automatic
   upgrades (or as a minimum allow security updates).

## Microsoft Office Apps

1. Go to https://www.office.com and sign in using your university email.
   You will be prompted to enter LUCAT credentials and thereafter
   taken to "Office 365" which is Microsoft's online version of office.
   Navigate to "Install Office Apps", download and install.

2. Once installed, accept all software updates if any, and also allow
   office to automatically download updates.

## Apple's developer tools

This is needed to further install compilers (C++, fortran etc.) and a large
variety of UNIX command line tools.

1. Install Xcode from the App Store (top-left corner in Finder) and wait for it to finish (may take a while!)

2. Open a Terminal (`Applications/Utilities/Terminal.app`) and enter
   the following which will download and install additional tools:
   ~~~ bash
   xcode-select --install
   ~~~

3. Open Xcode (`Applications/Xcode.app`) and accept the licence agreement.

## Python

Python is already installed on macOS or via macports (see below). However, a convenient way of managing packages and environments is via _Anaconda_.
Download from https://conda.io/miniconda.html (Python 3+, 64-bit) and install from a Terminal:

~~~ bash
chmod a+x ./Miniconda3-latest-MacOSX-x86_64.sh # make executable
./Miniconda3-latest-MacOSX-x86_64.sh # start; follow instructions.
~~~

## LaTeX typesetting

1. Go to http://www.tug.org/mactex and follow the link "Download MacTeX"

## Xquartz Windows manager (X11)

If you plan to use unix tools, MacPorts for example (see below), it is advised
to install an X11 windows manager. Go to https://www.xquartz.org and
download and install.

## Homebrew package manager

Homebrew is other package manager for installing unix command line tools and require Xcode (see above).

1. Install by running a single command line, pasted from the Homebrew frontpage, https://brew.sh

2. Search and install for packages using `brew search <package>` and `brew install <package>

Brew can also be used to install MacOS applications such as Firefox, Skype, Spotify etc.

### (MacPorts package manager)

As an alternative to brew, you may use macports which require Xcode (see above).

1. Go to https://www.macports.org/install.php and download to version
   matching your macOS version. Double-click in the installer.

2. One installed, you may search for and install tools from a Terminal.
   For example:
   ~~~ bash
   port search grace
   sudo port install grace
   sudo port install coreutils grace gawk wget cmake vim
   ~~~

## Cloud storage and backup:

Box is a service very similar to DropBox for online storage. By default LU employees have 20 GB of free storage and the service is security approved by the university (_Dropbox is not_). If you need to expand the disk space, simply call LDC service desk (phone 29000) and give them your LUCAT id and the space you need. For laptops, it makes no sense to expand the capacity with more than the laptop disk size, i.e. typically 128 or 256 GB.

To get started with Box:

1. Login to Box with LUCAT credentials from https://lu.account.box.com/login
2. Navigate to the "Apps" menu (top, right corner); then look for "Box Sync for Mac". Alternatively, this [link](https://app.box.com/settings/sync) may take you there directly.
3. Download, install, then open Box Sync.
4. Login with your university email and follow the instructions.

Once installed, you will have a new folder called "Box Sync" in your top-level user directory. All files placed here will be automatically synced to Box and _vice versa_. For example, you could install Box Sync on multiple computers and they will all be synched automatically. From the Box website you have access to version history of your files as well as the possibility to restore deleted files.

Finally, Box integrates with Microsoft's Office 360 (see above) and you can edit Word, Excell files etc. on Box directly from a web-browser without any additional software installed (for example from Linux). 

## Free access to Matlab, Maple, Comsol etc.

Login and download using LUCAT credentials at http://program.ddg.lth.se

## Printers

### General printing at LU

The large Canon printer on 2nd floor, shared between physical chemistry and theoretical chemistry, can be used only through the LU printing system PaperCut [(instructions here)](http://www.print.lu.se/english/papercut/). For every print you will need to use your access card at the printer. Employed staff pay no charge.

### HP LaserJet 500 (3rd floor)

1. Make sure you're logged into Apple App Store (top left corner menu item in Finder) using your Apple ID.
   This step may be required for system preferences to automatically download the required drivers.

2. Add manually in manually in System Preferences->Printers->Address:

       http://130.235.1.116 (HP JetDirect)
       
3. Add-ons: Duplex unit (twosided printing)

## More help?

Once the above is complete, contact M.L. if you need additional help.
