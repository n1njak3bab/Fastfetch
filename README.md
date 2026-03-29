<img width="1234" height="737" alt="Kuvakaappaus_20260328_224406" src="https://github.com/user-attachments/assets/087970e4-2fde-4a4a-b0a2-2badbdc43d7f" />

Install

home/.config/fastfetch/config.jsonc

```bash

hahaha
{
    "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/master/doc/json_schema.json",
    "logo": {
        "type": "small",
        "source": "arch", // search for logos: fastfetch --list-logos or --print-logos
        "color": {
            "1": "blink_cyan",
            "2": "blink_blue"
        },
        "padding": {
            "top": 7,
            "left": 5,
            "right": 5
        }
    },
    "display": {
        "bar": {
            "char": {
                "total": "─"
            },
            "color": {
                "border": "light_cyan",
                "total": "light_cyan"
            },
            "width": 10
        },
        "percent": {
            "type": 3,
            "ndigits": 2
        },
        "key": {
            "width": 16
        },
        "separator": "",
        "color": {
            "title": "magenta",
            "output": "light_cyan"
        }
    },
    "modules": [
        "break",
        {
            "type": "title",
            "key": "  ",
            "keyWidth": 4,
            "keyColor": "magenta",
            "color": {
                "at": "magenta"
            }
        },
        {
            "type": "datetime",
            "key": " ",
            "format": " 󰃮 {1}-{4}-{10} {14}:{18}:{20} ({22})"
        },
        "break",
        {
            "type": "custom",
            "key": "╭─System─────┬───────────────────────────────────────────────────╮",
            "keyColor": "magenta"
        },
        {
            "type": "host",
            "key": "├╴󰌢 PC       │",
            "keyColor": "magenta"
        },
        {
            "type": "os",
            "key": "├╴ OS       │",
            "keyColor": "magenta"
        },
        {
            "type": "wm",
            "key": "├╴ WM       │",
            "keyColor": "magenta"
        },
        {
            "type": "lm",
            "key": "├╴󰧨 LM       │",
            "keyColor": "magenta"
        },
        {
            "type": "kernel",
            "key": "├╴ Kernel   │",
            "keyColor": "magenta"
        },
        {
            "type": "bios",
            "key": "├╴ BIOS     │",
            "keyColor": "magenta"
        },
        {
            "type": "packages",
            "key": "├╴󰏖 Packages │",
            "keyColor": "magenta"
        },
        {
            "type": "font",
            "key": "├╴ Font     │",
            "keyColor": "magenta"
        },
        {
            "type": "cursor",
            "key": "├╴󰆿 Cursor   │",
            "keyColor": "magenta"
        },
        {
            "type": "uptime",
            "key": "├╴ Uptime   │",
            "keyColor": "magenta"
        },
        {
            "type": "command",
            "key": "├╴󱦟 OS Age   │",
            "keyColor": "magenta",
            "text": "birth_install=$(stat -c %W /); current=$(date +%s);    days_difference=$(( (current - birth_install) / 86400 )); echo $days_difference days"
        },

        {
            "type": "custom",
            "key": "╰────────────┴───────────────────────────────────────────────────╯",
            "keyColor": "magenta"
        },
        {
            "type": "custom",
            "key": "╭─Terminal───┬───────────────────────────────────────────────────╮",
            "keyColor": "magenta"
        },
        {
            "type": "shell",
            "key": "├╴ Shell    │",
            "keyColor": "magenta"
        },
        {
            "type": "terminal",
            "key": "├╴ Terminal │",
            "keyColor": "magenta"
        },
        {
            "type": "terminalfont",
            "key": "├╴ Font     │",
            "keyColor": "magenta"
        },
        {
            "type": "terminalsize",
            "key": "├╴󰘖 Size     │",
            "keyColor": "magenta",
            "format": "{1} colums × {2} rows ({3}px × {4}px)"
        },
        {
            "type": "custom",
            "key": "╰────────────┴───────────────────────────────────────────────────╯",
            "keyColor": "magenta"
        },
        {
            "type": "custom",
            "key": "╭─Hardware───┬───────────────────────────────────────────────────╮",
            "keyColor": "magenta"
        },
        {
            "type": "display",
            "key": "├╴󰍹 Display  │",
            "keyColor": "magenta",
            "format": "{1}×{2}, {3}Hz [{7}]"
        },
        {
            "type": "cpu",
            "key": "├╴ CPU      │",
            "keyColor": "magenta",
            "format": "{1} [{3} cores]"
        },
        {
            "type": "gpu",
            "key": "├╴󰾲 GPU      │",
            "keyColor": "magenta"
        },
        {
            "type": "memory",
            "key": "├╴ RAM      │",
            "keyColor": "magenta"
        },
        {
            "type": "disk",
            "key": "├╴ Disk     │",
            "keyColor": "magenta",
            "format": "{13} {1} / {2} ({3})"
        },
        {
            "type": "battery",
            "key": "├╴ Battery  │",
            "keyColor": "magenta",
            "format": "{10} {4} ({5})"
        },
        {
            "type": "custom",
            "key": "╰────────────┴───────────────────────────────────────────────────╯",
            "keyColor": "magenta"
        },
        {
            "type": "colors",
            "key": "╭─Media──────┬───────────────────────────────────────────────────╮",
            "keyColor": "magenta",
            "symbol": "diamond"
        },

        {
            "type": "player",
            "key": "├╴󰥠 Player   │",
            "keyColor": "magenta"
        },
        {
            "type": "sound",
            "key": "├╴󰋋 Sound    │",
            "keyColor": "magenta",
            "format": "{5} {3} ({2:20})"
        },
        {
            "type": "custom",
            "key": "╰────────────┴───────────────────────────────────────────────────╯",
            "keyColor": "magenta"
        }
    ]
}
