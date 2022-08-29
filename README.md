# Screenshoot Imgur

Full feature screenshot tool for wayland compositor.

![screenshot](https://i.imgur.com/JK9ADn2.png)


## Requiremnets

1. Python 3.6 or higher
2. [grim](https://archlinux.org/packages/community/x86_64/grim/) for screenshot
3. [slurp](https://archlinux.org/packages/community/x86_64/slurp/) for display geomety selection
4. [libnotify](https://archlinux.org/packages/extra/x86_64/libnotify/) for notification
5. [wl-clipboard](https://archlinux.org/packages/community/x86_64/wl-clipboard/) for clipboard

## Features

1. Delay when taking screnshoot
2. Desktop Notification
3. Full window and partial selection
4. Upload to imgur
5. Copy screenshoot to clipboard
6. Logging imgur uploads


## Usages

To avoid upload limits please use your own imgur client id. Supply your client id on global environment variable.

`export IMGUR_CLIENT_ID=YOUR_CLIENT_ID`


All the screenshoots will be saved at `~/Pictures/screenshots`, ensure your directory is there.



Please use --help flag to explore more.

## Examples

Take shoot with notification and save to path:

`screenshoot --notify --action save --type static --path /path/to/save --name my_file_name`


Same as above but select screen part:

`screenshoot --notify --action save --type select --path /path/to/save --name my_file_name`


Same as above but with 3 sec. delay:

`screenshoot --delay 3 --notify --action save --type select --path /path/to/save --name my_file_name`


Select screen, upload to imgur and keep a copy:

`screenshoot --notify --action imgur --type select --keep` (imgur url be copied to cliboard and details will be logged in a file.)


*Path and filename will be default path (~/Pictures/Wallpaper)*


Take, copy to clibboard and keep shoot to default path and do not notify: `screenshoot --action copy --type select --keep`


### __TODO__

