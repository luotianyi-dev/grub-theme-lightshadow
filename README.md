# LightShadow GRUB Theme

LightShadow is an animate GRUB theme in celebration of the 10th anniversary of the first Chinese VOCALOID character, Luo Tianyi.

This theme is named after the Luo's official birthday celebration song, [光与影的对白](https://b23.tv/BV1dZ4y1Y7bt).

This theme has two variants: **Light** and **Shadow**.

## Usage
```bash
mkdir -p /boot/grub/themes
git clone https://github.com/luotianyi-dev/grub-theme-lightshadow.git /boot/grub/themes/lightshadow
```

Based on your Linux distribution, the GRUB theme can be placed in one or more of the following directories:

 - `/usr/share/grub/themes/<theme-name>`
 - `/boot/grub/themes/<theme-name>`

Then, edit `/etc/default/grub`, set `GRUB_THEME=<theme-directory>/theme.txt`.

```
# For "Light" variant
echo 'GRUB_THEME="/boot/grub/themes/lightshadow/light/theme.txt"'  >> /etc/default/grub

# For "Shadow" variant
echo 'GRUB_THEME="/boot/grub/themes/lightshadow/shadow/theme.txt"' >> /etc/default/grub
```

Do not forget to regenerate GRUB configuration file after changing the theme:

```bash
# If you are using Ubuntu/Debian
update-grub

# For other distributions
grub-mkconfig -o /boot/grub/grub.cfg
```

Congratulations! You have successfully installed the theme. Reboot your computer to see the effect.

## License
This project is licensed under the `GPL-3.0-only` license with exceptions:

Files named `background.png` is illustrated by [TID](http://pixiv.net/users/418969) and should be used in non-commercial purposes.
See [Vsinger Copyright Agreement (Chinese Only)](https://vsinger.com/aboutus#版权说明) for details.
