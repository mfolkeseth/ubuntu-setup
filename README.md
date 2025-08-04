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
