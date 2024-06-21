# Catppuccin GRUB Theme

How to configure GRUB Catppuccin theme:

## Installation Steps

### 1. Copy the Theme Folder

Copy the `catppuccin-mocha-grub-theme` folder to the GRUB themes directory.

```bash
sudo cp -r catppuccin-mocha-grub-theme /usr/share/grub/themes/
```

### 2. Update GRUB Configuration

Add the content of `grub` to the GRUB configuration directory.

`Note: Directly copying file is not recommended, it is better to edit theme yourself without changing anything else in config`
```bash
sudo cp grub /etc/default/
```

#### Ensure that your `grub` file contains the following configuration

```ini
GRUB_THEME="/usr/share/grub/themes/catppuccin-mocha-grub-theme/theme.txt"
```
### 3. Update GRUB

To update/apply the grub config, you can use the following:

```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

Your GRUB should now be using the Catppuccin theme!
