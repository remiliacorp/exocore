---
published: true
topic:
subtitle:
date: 2022-09-26
tags: 
---

# Changing some test data

## Change your Username and Homepage ( test 2 )
Navigate to `/exocore/data/user.yml`. Open the file in any text-editor (e.g. Notepad or TextEdit) and look for `user_name: Remilia Corporation`. Change this to whatever name you want to appear on the left sidebar.

## Change your Homepage Content

In the same `/exocore/data/user.yml` file, you will also see `welcome_header` and `welcome_subtitle`. These control the title and subtitle that appear on your homepage.

On the root folder you will find `index.md`, this can be edited like any other article as your homepage with the addition of the title and header from the `user.yml` file. Make sure you keep the following frontmatter at the top of the markdown file: 

```
---
layout: home
title: home
---
```

## Change your Profile Picture

The profile picture that appears on the left sidebar is located at `assets/img/pfp.png`, you can replace this file with any .png. Note that it will be resized into a square. 

## Change your Social Media Card Image
The social media card that appears when your site is linked on social media sites like Twitter, Facebook, etc. is located at `assets/img/card.png`, you can replace this file with any .png. Note that a dimension of 1200x630 is recommended.

Make sure the site's url is changed in `/_config.yml` in the next step for this image to appear.

## Change your Site's Title and URL 
Navigate to ```/_config.yml``` to change the Title and URL of your exocore. All other settings can be left as is.

## Change the Theme
The Exocore ships with multiple themes to choose from. Navigate to `/styles.scss` and look for the line that says `//Uncomment one of the following lines to choose a theme:`. To select a theme, remove `//` from the line of the theme you want to try, and add `//` to the previously active theme ("yotsuba" by default).

## Optional: Password Protection

You can add simple password protection by going to your Netlify account, entering your site, going to `Settings > Build & Deploy > Build Settings > Edit Settings` and changing `Build commannd` from the default `bundle exec jekyll build` to: 
``jekyll build && npx staticrypt _site/index.html P@SSW0RD -o _site/index.html``

This will password protect the homepage with `P@SSWORD` as the password -- you can change this to anything you'd like. Note that this will only protect the homepage, users will be able to directly link to any other page and have access to the whole site.

---

Move on to [[Using your Exocore]] for further guidance.

