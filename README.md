# org.gtk.Gtk3theme.Breeze
### Workarounds
- Using a custom color scheme and accent color on KDE Plasma. Requires restarting app after changing color scheme/accent settings for it to apply. Related issue [#3901](https://github.com/flatpak/flatpak/issues/3901). Note: This will also expose the GTK's bookmarks and [servers](https://help.gnome.org/admin/system-admin-guide/stable/network-server-list.html.en) files under ~/.config/gtk-3.0/ if they are present.
  ```sh
  flatpak override --user --filesystem=xdg-config/gtk-3.0:ro
  ```
