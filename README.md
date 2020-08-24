![logo](static/img/icon.svg)

# Ficurinia

A prickly blog theme for Hugo

# [Demo](https://gabmus.org)

[Code for the demo website](https://gitlab.com/gabmus/gabmus.gitlab.io) (really my personal website)

# Customization

These are some parameters you can use in your `config.toml` to customize Ficurinia:

```toml
theme = "hugo-ficurinia"

title = "My nice blog"
copyright = "Some copyright notice"

paginate = 5  # number of articles per page in the index


[params]
    logo = "/images/mylogo.png"
    favicon = "/images/myfavicon.png"
    showTags = true  # show the Tags menu item; default true
    showRss = true  # show the link for the RSS feed; default true

    # enable comments support with commento using the script from your server
    commento = "https://example.com/js/commento.js"

    # the links array shows links with icons (if explicitly supported)
    # it's an array of arrays containing two strings: name and link
    # the supported icons are:
    #    gitlab
    #    gnome
    #    youtube
    #    email
    #    twitter
    #    instagram
    #    facebook
    #    github
    #    linkedin
    #    telegram
    #    phone
    #    rss
    links = [
        ["GitLab", "https://gitlab.com/gabmus"],
        ["GNOME", "https://gitlab.gnome.org/gabmus"],
        ["YouTube", "https://youtube.com/TechPillsNet"],
        ["Email", "mailto:gabmus@disroot.org"]
    ]

    # you can customize all of the colors in this theme
    # the values shown are the defaults
    backgroundColor = "#242629"
    foregroundColor = "white"
    dimForegroundColor = "#bababa"
    strokeColor = "#4f4f4f"
    accentColor = "#db5793"
```

# Does *Ficurinia* mean anything?

It's Sicilian for Indian fig, also known as prickly pear cactus.
