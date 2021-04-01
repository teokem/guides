# Apple M1 Compatibility

List of tested software on Apple M1. If not otherwise stated, all applications run native ARM code. Intel applications are silently emulated and a user will not notice this, except for demanding computations.

- [x] Microsoft office
- [x] Zoom (`brew install --cask zoom`)
- [x] Miniconda (x86)
- [x] Homebrew (x11, xmgrace, c++ compilers, emacs etc)
- [x] MacTex (x86, port on it's way)
- [x] gfortran (`brew install gcc`. May require `xcode-build --install` between MacOS updates)
- [x] Box Drive ([beta version](https://support.box.com/hc/en-us/community/posts/360051416514/comments/1500000521902) exists. Have not yet tried and the security of MacOS is reduced.)
- [x] Box Sync (x86, avoid this and use "Box Drive" if you can)
- [x] Faunus simulation software
- [x] Apple software (Final cut, compressor, motion, keynote etc.)
- [x] Browsers: Safari, Firefox, Brave
- [x] JetBrains CLion IDE
- [x] LibreOffice (x86, `brew install --cask libreoffice`)
- [x] Emacs (download [here](https://emacsformacosx.com/tips) and see the Tips section for running from command line)
- [x] Pymol (`conda install -c schrodinger pymol`. Starts a 30 day trial, whereafter a license is required)
- [ ] Molden (how can this be downloaded? if an x86 executable exists, it should run through Rosetta if X11 is installed)

## General tips

- Always start setting up by install Apple's Xcode and command line tools (remember `xcode-select --install`)

- If you intend to use X11 applications, also install `XQuartz` using brew; see below.

- Use only **Homebrew** as package manager. **Avoid** installing MacPorts or software manually. If you do anyways, make sure
the brew directory (`/opt/homebrew/bin`) is first in your PATH variable.

- Many MacOS applications can be installed with the `--cask` keyword from the command line with brew:
  ~~~ bash
  brew search <some_package>
  brew install --cask xquartz firefox libreoffice zoom
  ~~~

- For all Python related stuff, install [Miniconda](https://conda.io/en/master/miniconda.html), then install with `conda install ...`
  Install miniconda after you have install brew.

- On the M1 you can run x86 binary command line tools through Rosetta emulation. This is done automatically and in the background.
  To see if a file is arm or x86, use `file <executable>`


