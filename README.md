# org.gtk.Gtk3theme.Breeze
### Workarounds
- Using a custom color scheme and ascent color on KDE Plasma. Requires restarting app after changing color scheme/ascent settings for it to apply. Related issue [#3901](https://github.com/flatpak/flatpak/issues/3901).
  ```sh
  flatpak override --user --filesystem=xdg-config/gtk-3.0/settings.ini:ro \
  --filesystem=xdg-config/gtk-3.0/gtk.css:ro \
  --filesystem=xdg-config/gtk-3.0/colors.css:ro
  ```
