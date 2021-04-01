# Regolith

https://regolith-linux.org/

##Config
[Docs](https://regolith-linux.org/docs/getting-started/configuration/)

`~/.config/regolith/Xresources`

```
i3-wm.bar.position: top
i3-wm.bar.trayoutput:primary
i3-wm.gaps.inner.size: 8
i3-wm.gaps.outer.size: 4

i3-wm.workspace.01.name: 1:<span font_desc='JetBrains Mono Medium 13'> 1: coms </span>
workspace "$ws1" output eDP-1
i3-wm.workspace.02.name: 2:<span font_desc='JetBrains Mono Medium 13'> 2: coding </span>
workspace "$ws2" output HDMI-2
i3-wm.workspace.03.name: 3:<span font_desc='JetBrains Mono Medium 13'> 3: coding </span>
i3-wm.workspace.03.name: 3:<span font_desc='JetBrains Mono Medium 13'> 4: focus </span>
i3-wm.workspace.05.name: 5:<span font_desc='JetBrains Mono Medium 13'> 5: postman </span>
i3-wm.workspace.11.name: 11:<span font_desc='JetBrains Mono Medium 13'> 11: private </span>
i3-wm.workspace.12.name: 12:<span font_desc='JetBrains Mono Medium 13'> 12: leetcode </span>
i3-wm.workspace.13.name: 13:<span font_desc='JetBrains Mono Medium 13'> 13: advent of code </span>
i3-wm.workspace.19.name: 19:<span font_desc='JetBrains Mono Medium 13'> 19: music </span>

i3-wm.floatingwindow.border.size: 3

for_window [class=”Slack”] move to workspace $ws1
for_window [class=”Evolution”] move to workspace $ws1

gnome.wallpaper: 

```



## List of installed packages

This was grabed retrospectively through `apt list | grep i3x` and `apt list | grep regolith`, 
so no need to install all these by hand, but might be useful if I'm looking for something that I used to have and didn't come as default. 

```
i3xrocks-battery/focal,now 3.5.7-1 amd64 [installed]
i3xrocks-battery/focal 3.5.7-1 i386
i3xrocks-bluetooth/focal 3.5.7-1 amd64
i3xrocks-bluetooth/focal 3.5.7-1 i386
i3xrocks-cpu-usage/focal,now 3.5.7-1 amd64 [installed]
i3xrocks-cpu-usage/focal 3.5.7-1 i386
i3xrocks-disk-capacity/focal 3.5.7-1 amd64
i3xrocks-disk-capacity/focal 3.5.7-1 i386
i3xrocks-focused-window-name/focal,now 3.5.7-1 amd64 [installed]
i3xrocks-focused-window-name/focal 3.5.7-1 i386
i3xrocks-info/focal 3.5.7-1 amd64
i3xrocks-info/focal 3.5.7-1 i386
i3xrocks-key-indicator/focal 3.5.7-1 amd64
i3xrocks-key-indicator/focal 3.5.7-1 i386
i3xrocks-keyboard-layout/focal 3.5.7-1 amd64
i3xrocks-keyboard-layout/focal 3.5.7-1 i386
i3xrocks-media-player/focal 3.5.7-1 amd64
i3xrocks-media-player/focal 3.5.7-1 i386
i3xrocks-memory/focal 3.5.7-1 amd64
i3xrocks-memory/focal 3.5.7-1 i386
i3xrocks-net-traffic/focal,now 3.5.7-1 amd64 [installed]
i3xrocks-net-traffic/focal 3.5.7-1 i386
i3xrocks-next-workspace/focal,now 3.5.7-1 amd64 [installed,automatic]
i3xrocks-next-workspace/focal 3.5.7-1 i386
i3xrocks-nm-vpn/focal 3.5.7-1 amd64
i3xrocks-nm-vpn/focal 3.5.7-1 i386
i3xrocks-openvpn/focal 3.5.7-1 amd64
i3xrocks-openvpn/focal 3.5.7-1 i386
i3xrocks-rofication/focal 3.5.7-1 amd64
i3xrocks-rofication/focal 3.5.7-1 i386
i3xrocks-temp/focal 3.5.7-1 amd64
i3xrocks-temp/focal 3.5.7-1 i386
i3xrocks-time/focal,now 3.5.7-1 amd64 [installed]
i3xrocks-time/focal 3.5.7-1 i386
i3xrocks-todo/focal 3.2.5-1ubuntu1 amd64
i3xrocks-todo/focal 3.2.5-1ubuntu1 i386
i3xrocks-volume/focal 3.5.7-1 amd64
i3xrocks-volume/focal 3.5.7-1 i386
i3xrocks-weather/focal 3.5.7-1 amd64
i3xrocks-weather/focal 3.5.7-1 i386
i3xrocks-wifi/focal 3.5.7-1 amd64
i3xrocks-wifi/focal 3.5.7-1 i386
i3xrocks/focal,now 1.3.5-1 amd64 [installed,automatic]
i3xrocks/focal 1.3.5-1 i386
regolith-i3xrocks-config/focal,now 3.5.7-1 amd64 [installed,automatic]
regolith-i3xrocks-config/focal 3.5.7-1 i386

fonts-jetbrains-mono/focal,focal,now 1.0.1-1regolith1 all [installed,automatic]
fonts-materialdesignicons-webfont/focal,now 1.6.50-3regolith3 amd64 [installed,automatic]
fonts-materialdesignicons-webfont/focal 1.6.50-3regolith3 i386
plano-theme/focal,focal 3.36-1-1regolith1 all
plymouth-theme-regolith/focal,focal 1.0.3-1 all
regolith-compositor-compton-glx/focal,now 1.1.0-1 amd64 [installed,automatic]
regolith-compositor-compton-glx/focal 1.1.0-1 i386
regolith-compositor-none/focal 1.0.3-1 amd64
regolith-compositor-none/focal 1.0.3-1 i386
regolith-compositor-picom-glx/focal 1.1.3-1 amd64
regolith-compositor-picom-glx/focal 1.1.3-1 i386
regolith-compositor-xcompmgr/focal 1.2.0-1 amd64
regolith-compositor-xcompmgr/focal 1.2.0-1 i386
regolith-default-settings/focal,now 1.0.3-1focal amd64 [installed,automatic]
regolith-desktop-complete/focal 2.110-1focal amd64
regolith-desktop-minimal/focal 2.110-1focal amd64
regolith-desktop-mobile/focal 2.110-1focal amd64
regolith-desktop-standard/focal 2.110-1focal amd64
regolith-desktop/focal,now 2.110-1focal amd64 [installed]
regolith-ftue/focal,now 1.1.0-1 amd64 [installed,automatic]
regolith-ftue/focal 1.1.0-1 i386
regolith-gdm3-theme/focal 2.0.0-1ubuntu1~ppa1 amd64
regolith-gdm3-theme/focal 2.0.0-1ubuntu1~ppa1 i386
regolith-gnome-flashback/focal,now 2.6.2-1 amd64 [installed,automatic]
regolith-gnome-flashback/focal 2.6.2-1 i386
regolith-i3-gaps-config/focal,now 2.8.4-1 amd64 [installed,automatic]
regolith-i3-gaps-config/focal 2.8.4-1 i386
regolith-i3xrocks-config/focal,now 3.5.7-1 amd64 [installed,automatic]
regolith-i3xrocks-config/focal 3.5.7-1 i386
regolith-lightdm-config/focal 1.0.6-1 amd64
regolith-lightdm-config/focal 1.0.6-1 i386
regolith-look-ayu-dark/focal 2.6.16-1 amd64
regolith-look-ayu-dark/focal 2.6.16-1 i386
regolith-look-ayu-mirage/focal 2.6.16-1 amd64
regolith-look-ayu-mirage/focal 2.6.16-1 i386
regolith-look-ayu/focal 2.6.16-1 amd64
regolith-look-ayu/focal 2.6.16-1 i386
regolith-look-cahuella/focal 2.6.16-1 amd64
regolith-look-cahuella/focal 2.6.16-1 i386
regolith-look-dracula/focal 2.6.16-1 amd64
regolith-look-dracula/focal 2.6.16-1 i386
regolith-look-gruvbox/focal 2.6.16-1 amd64
regolith-look-gruvbox/focal 2.6.16-1 i386
regolith-look-lascaille/focal,now 2.6.16-1 amd64 [installed,automatic]
regolith-look-lascaille/focal 2.6.16-1 i386
regolith-look-nord/focal 2.6.16-1 amd64
regolith-look-nord/focal 2.6.16-1 i386
regolith-look-pop-os/focal 2.6.16-1 amd64
regolith-look-pop-os/focal 2.6.16-1 i386
regolith-look-solarized-dark/focal,now 2.6.16-1 amd64 [installed]
regolith-look-solarized-dark/focal 2.6.16-1 i386
regolith-look-ubuntu/focal,now 2.6.16-1 amd64 [installed]
regolith-look-ubuntu/focal 2.6.16-1 i386
regolith-rofi-config/focal,now 1.3.1-1 amd64 [installed,automatic]
regolith-rofi-config/focal 1.3.1-1 i386
regolith-rofication/focal,now 1.3.1-1 amd64 [installed,automatic]
regolith-rofication/focal 1.3.1-1 i386
regolith-st/focal 0.8.2-1ubuntu20ppa5 amd64
regolith-st/focal 0.8.2-1ubuntu20ppa5 i386
regolith-styles/focal,now 2.6.16-1 amd64 [installed,automatic]
regolith-styles/focal 2.6.16-1 i386
regolith-system/focal 1.4.0.4-1 amd64
regolith-system/focal 1.4.0.3-1 i386
regolith-todo/focal 1.2.1-1 amd64
regolith-todo/focal 1.2.1-1 i386
regolith-unclutter-xfixes/focal,now 1.5-2 amd64 [installed,automatic]
regolith-unclutter-xfixes/focal 1.5-2 i386
ubiquity-slideshow-regolith/focal,focal 138.5-ubuntu1~regolith1 all

```