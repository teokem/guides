# Setting up new macs

Instructions for setting up new macOS system at teokem; please follow in the presented order.

## Basic setup and updating

1. Power on the laptop and follow instructions for creating a user account.

2. When asked, create an iCloud account if you do not already
   have one. This is required to install i.e. Apple's developer tools.

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
./Miniconda3-latest-MacOSX-x86_64.sh # start; follow instatruction
~~~

## LaTeX typesetting

1. Go to http://www.tug.org/mactex and follow the link "Download MacTeX"

## Xquartz Windows manager (X11)

If you plan to use unix tools, MacPorts for example (see below), it is advised
to install an X11 windows manager. Go to https://www.xquartz.org and
download and install.

## MacPorts package manager

Macports is a package manager for installing unix command line tools and require Xcode (see above).

1. Go to https://www.macports.org/install.php and download to version
   matching your macOS version. Double-click in the installer.

2. One installed, you may search for and install tools from a Terminal.
   For example:
   ~~~ bash
   port search grace
   sudo port install grace
   sudo port install coreutils grace gawk wget cmake vim
   ~~~

## Cloud storage and backup: Box/Dropbox

Box and Dropbox provide similar services for online storage and both have free options. In particular, all LU employees have 20 GB of free storage on Box which is also the only of the two that is security approved by the university.

1. Download "Box sync" from https://sites.box.com/sync4 and once installed, login using your university email/LUCAT credentials (no need to create an account)

## Free access to Matlab, Maple, Comsol etc.

Login and download using LUCAT credentials at http://program.ddg.lth.se

## Printers

### Canon Image Runner C5560i (2nd floor)

1. Download and install [drivers](https://www.canon.co.uk/support/products/imagerunner/imagerunner-advance-c5560i.aspx?type=drivers&os=MAC%20OS%20X).

2. Add manually in System Preferences->Printers->Address:

       socket://130.235.71.66:9100 (socket/jetdirect)

3. Add-ons: High capacity casette, feed unit-a1, stable finisher-Y1

### LaserJet 500 (3rd floor)

1. Make sure you're logged into Apple App Store (top left corner menu item in Finder)

2. Add manually in manually in System Preferences->Printers->Address:

       http://130.235.1.116 (HP JetDirect)

# Backup and more help?

Once the above is complete, contact M.L. if you need to backup to Time Machine, wired ethernet access etc.
