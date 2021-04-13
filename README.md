![logo](static/img/icon.svg)

# Ficurinia

A prickly blog theme for Hugo

![](images/tn.png)

# [Demo](https://gabmus.org)

[Code for the demo website](https://gitlab.com/gabmus/gabmus.gitlab.io) (really my personal website)

# Customization

## Configuration

These are some parameters you can use in your `config.toml` to customize Ficurinia:

```toml
theme = "hugo-ficurinia"

title = "My nice blog"
copyright = "Some copyright notice"

paginate = 5  # number of articles per page in the index
summaryLength = 70  # number of words for article summaries


[params]
    author = "Gabriele Musco"
    logo = "/images/mylogo.png"
    favicon = "/images/myfavicon.png"
    showTags = true  # show the Tags menu item; default true
    showRss = true  # show the link for the RSS feed; default true
    
    imageInArticlePreview = false  # show images in article preview; default false

    navtype = "standard"  # changes the style of the pagination, available styles are: "standard", "circle"
    fontFamily = "JetBrains Mono"  # changes the font, default "JetBrains Mono"
    monospaceFontFamily = "JetBrains Mono"  # changes the monospace font for code, default "JetBrains Mono"
    contentWidth = "1000px"  # maximum width of the site content, css syntax

    discreteCards = false  # enable discrete card style; default false
    gridView = false  # show post list as a grid. goes well with discreteCards
    highlightBgColor = "#34363b";  # card and circle navigation background color for discrete card mode

    enableSearch = true  # enable search page

    # enable comments support with commento using the script from your server
    commento = "https://example.com/js/commento.js"

    # enable analytics using Plausible
    plausibleScriptUrl = "https://something.com/..."
    plausibleDomain = "gabmus.org"

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

    # redirect to baseURL if current URL host doesn't match
    # useful if deploying in gitlab pages with custom domain and don't want
    # the username.gitlab.io/website url to persist
    forceRedirect = false

    infiniteScrolling = false  # activates infinite scrolling instead of regular pagination

# this section is necessary if you want infinite scrolling
# it allows to output the article list as paged JSON so that "pages" can be retrieved via javascript
[outputs]
    home = ["HTML", "JSON"]
```

## Inject custom content

Ficurinia supports injecting custom content into the theme. There are several files you can create in `layouts/partials/inject` that will be included inside the theme in different places.

| Partial | Placement |
|---------|-----------|
| `layouts/partials/inject/body.html` | Before closing the `body` tag |
| `layouts/partials/inject/content-after.html` | After a post or page content |
| `layouts/partials/inject/content-before.html` | Before a post or page content |
| `layouts/partials/inject/footer.html` | At the beginning of the footer |
| `layouts/partials/inject/head.html` | Before closing the `head` tag |
| `layouts/partials/inject/header-after.html` | Before closing the header |
| `layouts/partials/inject/header-before.html` | At the beginning of the header |

# Does *Ficurinia* mean anything?

It's Sicilian for Indian fig, also known as prickly pear cactus.
