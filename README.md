# CTF-Generator

### Hide Grub

GRUB_TIMEOUT=0

GRUB_TIMEOUT_STYLE=hidden

GRUB_HIDDEN_TIMEOUT=0

GRUB_HIDDEN_TIMEOUT_QUIET=true

### On Debian/Ubuntu and derivatives:
sudo update-grub

### On Fedora/Arch:
sudo grub2-mkconfig -o /boot/grub2/grub.cfg
