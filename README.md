# LightShadow: 洛天依 10 周年纪念 GRUB 主题

LightShaodw 是一个以洛天依 10 周年纪念主题 [光与影的对白](https://b23.tv/BV1dZ4y1Y7bt) 为素材制作的 GRUB 主题。

LightShadow 分为 **`light` (光)** 和 **`shadow` (影)** 两个版本。均使用 [TID](http://pixiv.net/users/418969) 绘制的插画作为素材。

## 下载与安装
运行以下命令下载主题：
```bash
mkdir -p /boot/grub/themes
git clone https://github.com/luotianyi-dev/grub-theme-lightshadow.git /boot/grub/themes/lightshadow
```

然后，您需要配置您的 GRUB 配置。根据您的 Linux 发行版不同，您的 GRUB 配置可能位于不同位置。一般来说，配置位于 `/etc/default/grub`。若您的 Linux 发行版使用不同的位置，请修改以下命令中的配置文件路径。

```bash
# 「光」版本
echo 'GRUB_THEME="/boot/grub/themes/lightshadow/light/theme.txt"'  >> /etc/default/grub

# 「影」版本
echo 'GRUB_THEME="/boot/grub/themes/lightshadow/shadow/theme.txt"' >> /etc/default/grub
```

最后，更新 GRUB 配置文件：
```bash
# Ubuntu/Debian 系统
update-grub

# 其他发行版
grub-mkconfig -o /boot/grub/grub.cfg
```

现在，您可以**重启**您的计算机。您应当可以看到 LightShadow 已经安装成功。

## 许可
此项目基于 [TID](http://pixiv.net/users/418969) 绘制的「光与影的对白」插画制作，该作品可以推定为 Vsinger 官方作品，需遵守 [Vsinger 同人使用规约](https://vsinger.com/aboutus#版权说明)。

项目作者对此项目不声明除要求署名外的任何权利。若您转载、修改或向他人提供此项目，您应当知会您的受众此项目的许可信息，包括项目作者、项目地址和署名信息和相关的同人创作规约。
