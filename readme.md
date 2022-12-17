# Swaymsg-treefetch: Simple bash scripts to fetch wanted info using swaymsg

### Requirements
- Window Manager: sway
- Dependencies: swaymsg, jshon

## Swaymsg-rectfetcher

Fetch rect info of window with app_id.

This bash script could get the rect (i.e. absolute coordinates and size) info of the window with specified app_id (the first argument) in SwayWM.

 If multiple window matches, the focused window will be selected. 
 If no one is focused, the first one will be selected.

 Remove every '#' before "$pecho" in the script file to get verbose output.

### Usage
```bash
 $ swaymsg-rectfetcher <app_id>
```

### Output format
```bash
 <x> <y> <width> <height>
```

## Swaymsg-rectfetcher

Fetch the app_id of focused window.

Remove every '#' before "$pecho" in the script file to get verbose output.

### Usage
```bash
 $ swaymsg-focusfetcher
```

### Output format
```bash
 <app_id>
```

## Examples
```bash
$ swaymsg-rectfetcher emacs
1080 1546 1800 374
$ swaymsg-focusfetcher
emacs
```
## LICENSE
MIT license
