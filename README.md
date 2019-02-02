## .i3status.conf

By default, i3status looks for configuration files in the following order:

* ~/.i3status.conf

* ~/.config/i3status/config (or $XDG_CONFIG_HOME/i3status/config if set)

* /etc/i3status.conf

* /etc/xdg/i3status/config (or $XDG_CONFIG_DIRS/i3status/config if set)

## config

The default config is located at `/etc/i3/config/`
Custom config files can be placed in `~/.i3/config` or `~/.config/i3/config`

Some of my custom changes include:

Swap the mouse buttons to be left handed:

    exec xmodmap -e "pointer = 3 2 1"

Change the movement keys to match vim:

    # change focus

    bindsym $mod+h focus left

    bindsym $mod+j focus down

    bindsym $mod+k focus up

    bindsym $mod+l focus right

Since $mod+h is now being used to move left, I needed a new key for horizontal split. I chose 'b' because it's fairly close to h, and next to 'v' (on qwerty).

Added a shortcut to a black lock screen:

    bindsym $mod+p exec i3lock -c 000000


