# Catppuccin SDDM Theme

How to configure SDDM catppuccin theme:

## Installation Steps

### 1. Copy the Theme Folder

Copy the `catppuccin` folder to the SDDM themes directory.

```bash
sudo cp -r catppuccin /usr/share/sddm/themes/
```

### 2. Update SDDM Configuration

Add the content of `10-theme.conf` to the SDDM configuration directory.

```bash
sudo cp 10-theme.conf /etc/sddm.conf.d/10-theme.conf
```

#### Ensure that your `10-theme.conf` file contains the following configuration

```ini
[Theme]
Current=catppuccin
```
### 3. Verification

To verify that the theme has been applied correctly, you can restart the SDDM service:

```bash
sudo systemctl restart sddm
```

Your SDDM should now be using the Catppuccin theme!