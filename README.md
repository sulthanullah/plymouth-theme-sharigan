
# Plymouth Theme Sharingan

![License](https://img.shields.io/github/license/sulthanullah/plymouth-theme-sharigan?style=flat-square)
![Stars](https://img.shields.io/github/stars/sulthanullah/plymouth-theme-sharigan?style=flat-square)
![Forks](https://img.shields.io/github/forks/sulthanullah/plymouth-theme-sharigan?style=flat-square)

A visually appealing Plymouth boot theme inspired by the iconic Sharingan from Naruto. Enhance your Linux startup experience with this anime-themed loading screen.

---

## Preview

**Sharingan Boot Animation:**

![Preview](https://raw.githubusercontent.com/sulthanullah/plymouth-theme-sharigan/refs/heads/main/preview/sharigan.gif)

---

## Installation

Follow these simple steps to install the Sharingan Plymouth theme on your Linux distribution:

1. Clone this repository:
   ```bash
   git clone https://github.com/sulthanullah/plymouth-theme-sharigan.git
   ```

2. Move to the cloned directory:
   ```bash
   cd plymouth-theme-sharigan
   ```

3. Copy the theme folder to Plymouth themes directory:
   ```bash
   sudo cp -r sg /usr/share/plymouth/themes/
   ```

4. Set Sharingan as your Plymouth theme:
   ```bash
   sudo plymouth-set-default-theme -R sg
   ```

5. Update initramfs:
   ```bash
   sudo update-initramfs -u
   ```

6. Reboot your system to enjoy the new theme!

---

## Compatibility

This theme is tested and works well on popular Linux distributions including:
- Ubuntu
- Debian
- Linux Mint
- Arch Linux
- Fedora
- Kali Linux (developed and tested on Kali Linux)

(Ensure Plymouth is installed on your system before proceeding.)

---

## Thank's to https://github.com/adi1090x


---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
