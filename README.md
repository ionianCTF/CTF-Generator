
# How to Completely Hide the GRUB Loader

## 1. Open Terminal

```bash
sudo nano /etc/default/grub
```

## 2. Edit the file with the following lines

Make sure these lines are either added or updated:

```bash
GRUB_TIMEOUT=0
GRUB_TIMEOUT_STYLE=hidden
GRUB_HIDDEN_TIMEOUT=0
GRUB_HIDDEN_TIMEOUT_QUIET=true
```

## 3. Update GRUB

- On **Debian/Ubuntu and derivatives:**

```bash
sudo update-grub
```

- On **Fedora/Arch:**

```bash
sudo grub2-mkconfig -o /boot/grub2/grub.cfg
```

## 4. Reboot

```bash
sudo reboot
```
