# ubuntu-setup

# Screen management

## xrandr

**Show screens**

```bash
xrandr | grep " connected " | awk '{ print$1 }'
```

**Rotate screen**

```bash
xrandr --output HDMI-0 --rotate right
```

# Sound

**PulseAudio**

```bash
sudo apt-get install pulseaudio pavucontrol playerctl
```

**Update config**

Add the following under volume control settings

```bash
bindsym XF86AudioPause exec playerctl play-pause
bindsym XF86AudioPlay exec playerctl play-pause
bindsym XF86AudioNext exec playerctl next
bindsym XF86AudioPrev exec playerctl previous
```


