# Screenshoot Imgur

Full feature screenshot tool for wayland compositor.

![screenshot](https://i.imgur.com/JK9ADn2.png)


## Requiremnets

1. Python 3.6 or higher
2. grim for screenshot
3. slurp for display geomety selection
4. libnotify for notification
5. wl-copy for clipboard

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



### __TODO__

