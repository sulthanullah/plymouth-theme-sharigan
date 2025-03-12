# Plymouth Theme Sharigan

What is plymouth?
Plymouth is a project from Fedora and now listed among the freedesktop.org's official resources providing a flicker-free graphical boot process. It relies on kernel mode setting (KMS) to set the native resolution of the display as early as possible, then provides an eye-candy splash screen leading all the way up to the login manager.

How to set it up?
follow this archwiki article to setup plymouth in archlinux or any other distro.

Clone : or you can clone this repository if you want -



How to use these theme?
follow the step below (I'm using archlinux here)-
# packages needed - plymouth, plymouth-x11, plymouth-plugin-script(fedora)

# after downloading or cloning themes, copy the selected theme in plymouth theme dir
sudo cp -r angular /usr/share/plymouth/themes/

# check if theme exist in dir
sudo plymouth-set-default-theme -l

# now set the theme (angular, in this case) and rebuilt the initrd
sudo plymouth-set-default-theme -R angular

# optionally you can test theme by running the script given in repo (plymouth-x11 required)
sudo ./showplymouth.sh 20
For debian(Ubuntu, Kubuntu) based distros-
# make sure you have the packages for plymouth
sudo apt install plymouth

# after downloading or cloning themes, copy the selected theme in plymouth theme dir
sudo cp -r angular /usr/share/plymouth/themes/

# install the new theme (angular, in this case)
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/angular/angular.plymouth 100

# select the theme to apply
sudo update-alternatives --config default.plymouth
#(select the number for installed theme, angular in this case)

# update initramfs
sudo update-initramfs -u
