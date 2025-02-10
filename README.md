# `org.gtk.Gtk3theme.Breeze`

### Workarounds

Using a custom color scheme and accent color on KDE Plasma requires restarting the app after changing the color scheme/accent settings for it to apply. The related issue is [#3901](https://github.com/flatpak/flatpak/issues/3901).

> [!NOTE]
> This will also expose the GTK's bookmarks and [servers](https://help.gnome.org/admin/system-admin-guide/stable/network-server-list.html.en) files under `$HOME/.config/gtk-3.0/` if they are present.

```sh
#!/usr/bin/env sh
flatpak override --system \
    --filesystem=xdg-config/gtk-3.0:ro \
    --filesystem=xdg-config/gtkrc-2.0:ro \
    --filesystem=xdg-config/gtk-4.0:ro \
    --filesystem=xdg-config/gtkrc:ro \
```

Superuser permission may be necessary.
