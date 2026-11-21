
# ***Anon-Scripts v4.0.1***
- Copyright (c) 2026 Archnon Project. All Rights Reserved.

## ***Features***

- Proxy support: Tor and i2pd.
- Firewall: nftables.
- Supported Systems for service: systemd, runit, open-rc.
- Supported Package managers: apt, pacman, dnf, yum, apk, zypper, emerge, xbps-install.
- Number of scripts: 4.
- Special support for Arch users: PKGBUILD and .pkg.tar.zst.
- Easy to use and dynamic.

## ***Creator***

- [@archnon-project](https://www.github.com/archnon-project) (archnon@protonmail.com)

## ***Installation (you can copy and paste the commands below)***

1. Clone this GitHub repository, right from your terminal:

```bash
  git clone https://github.com/archnon-project/anon-scripts/
```

2. Change your current position to inside the main directory:

```bash
  cd anon-scripts
```

3. Set right executable permissions to all files inside it:

```bash
   su && chmod +x * || chmod +x *
```

4. Run one of the scripts and let it handle all needed packages:

```bash
  ./archnon # or whatever
```

## ***Installation for Arch-based distros (a second way, this is optional but i recommend)***

1. Clone this GitHub repository, right from your terminal:

```bash
  git clone https://github.com/archnon-project/anon-scripts/
```

2. Change your current position to inside the main directory:

```bash
  cd anon-scripts
```

3. Build the package with makepkg (avoid deleting PKGBUILD):

```bash
   sudo -u $USER makepkg -f -si # replace $USER with a non-privileged local user.
```

4. Verify is installed:

```bash
  pacman -Qi archnon-project # it will show lot of information about this project
```
5. Test and let the scripts manage all dependencies alone:
```bash
  archnon --version # the same with: mars, neptune, saturn, uranus.
```

## ***License***
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/) 
* [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
