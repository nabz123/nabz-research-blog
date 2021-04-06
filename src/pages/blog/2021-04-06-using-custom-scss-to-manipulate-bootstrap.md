---
templateKey: blog-post
title: "Using custom SCSS to manipulate bootstrap "
date: 2021-04-06T08:18:09.012Z
description: How to change bootstrap default font-family.
featuredpost: true
featuredimage: /img/pin-transparent-images-png.png
tags:
  - scss
---
To manipulate out the box font family provided by bootrap (Reboot) you need to do the following steps

Import the font

```
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,700;0,900;1,900&display=swap');
```

Assign your imported font to a local variable

```
$heading-font: 'Merriweather', serif;
```

Then assign it to a certain class or id

```
.card-title{
    font-family: $heading-font;
    font-weight: bold;
}
```