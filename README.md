# The Fucking Docs

Basic Hugo theme for documentation style websites.

This template uses Bootstrap v5 and Bootstrap icons combined with the Bootswatch Flatly theme.


You can select a specific partial for branding, or use the default with a "title icon"
```toml
# in /config.toml
[params]
  # Set the title icon.
  title_icon = "book"

  # Set our own branding.
  brand_partial = "our-brand-logo.html"
```

```toml
logo_html = '<span class="text-primary">Hello</span><span class="text-secondary">World</span>'
```

Social media icons in the top right are menu based. If something doesn't have an icon, it defaults to the title. Only a limited set for now.
```toml
[menu]
  [[menu.social]]
    name = "github"
    url = "https://github.com/"

  [[menu.social]]
    name = "twitter"
    url = "https://twitter.com/"

  [[menu.social]]
    name = "slack"
    url = "https://slack.com/"

  [[menu.social]]
    name = "youtube"
    url = "https://youtube.com/"

  [[menu.social]]
    name = "youtube"
    url = "https://youtube.com/"
```


The footer menus are also just one menu (preferrably of exactly 3 items) with any number of child menu items.
```toml
[menu]
  [[menu.footer]]
    name = "Features"

  [[menu.footer]]
    name = "Resources"

  [[menu.footer]]
    name = "About"

  [[menu.footer]]
    name = "Team"
    parent = "About"

  [[menu.footer]]
    name = "Cool stuff"
    parent = "Features"

  [[menu.footer]]
    name = "Random feature"
    parent = "Features"

  [[menu.footer]]
    name = "Team feature"
    parent = "Features"

  [[menu.footer]]
    name = "Stuff for developers"
    parent = "Features"

  [[menu.footer]]
    name = "Another one"
    parent = "Features"

  [[menu.footer]]
    name = "Last time"
    parent = "Features"

  [[menu.footer]]
    name = "Resource"
    parent = "Resources"

  [[menu.footer]]
    name = "Resource name"
    parent = "Resources"

  [[menu.footer]]
    name = "Another resource"
    parent = "Resources"

  [[menu.footer]]
    name = "Final resource"
    parent = "Resources"

  [[menu.footer]]
    name = "Team"
    parent = "About"

  [[menu.footer]]
    name = "Locations"
    parent = "About"

  [[menu.footer]]
    name = "Privacy"
    parent = "About"

  [[menu.footer]]
    name = "Terms"
    parent = "About"
```