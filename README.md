# sharetags
Awesome WM plugin to share tags across multiple monitors

extracted into a deployabel submodule from (lammermann/awesome-configs)[https://github.com/lammermann/awesome-configs]

## Installation

    $ git clone git://github.com/seagoj/sharetags.git ~/.config/awesome/sharetags

## Configuration

### ~/.config/awesome/rc.lua

    -- Share tags on multiple screens
    local sharetags = require("sharetags")

    tags = {
        names = { "main", "www", "office", "virtual", "eda", "cad", "screen", "media", 9 },
        layout = { layouts[2], layouts[4], layouts[1], layouts[2], layouts[12],
                   layouts[4], layouts[11], layouts[2], layouts[1]
        }
    }
    tags = sharetags.create_tags(tags.names, tags.layout)

