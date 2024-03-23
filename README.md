<!--README.md file for Github Repo-->
# 3dIconify -- Web App Icon Generation.
Build Icons for your Web App using the [3dIcons](https://github.com/realvjy/3dicons) source.

Generates smaller icons on an optionally transparent background using the
requested 3dIcon resource(s).

Supports resource naming prefix, and icon name conversion to meet specific
project resource naming standards.

## This project enables developers to:
1. Work with a professionally designed open source icon set.
1. Scale icons to the size requirements of their project.
1. Spend less time installing npm compoents or learning yet another REST API just to get icons.
1. Spend more time writing code. :smile:

# History:
While working on [BASE](https://github.com/NathanGibbs3/BASE), we needed to
standardize the app's iconography.

## What we had, Icons:
1. Designed to varying specs & standards.
2. With no consistent resource naming convention.

## What we needed, Icons:
1. Designed to the same specs & standards.
1. Compatible with older Web Browsers, *PNGs **NOT** SVGs*.
1. That could scale to different sizes and still look good.
1. Released under an Open Source License.
   1. So we can release them as part of our project.
   1. So we can modify them if needed.

The [3dIcons](https://github.com/realvjy/3dicons) project met all the criteria.
We developed a custom tool, that transforms the icons we need to use in BASE,
to specific specs and stores them according to our resource naming standrads.

## This project:
`3dIconify`, the open source version of the custom tool, takes a project file,
the 3dIcons source; and builds an icon set, with the requested icon size,
background transparency, and naming scheme.

# Usage:
Command Line Options, *great for one off testing*, are space sepearated; and
support a subset of what can be done in a 3dIconify project file.

## Options:
1. Location of 3dIcons or 3dIconify project file. ( defaults to 3dIcons )
   1. 3dIconify project files have the extension .3dicp
   1. See: `docs/BASE.example.3dicp` for more informarion.
1. Location of generated Icons. ( defaults to Icons )
1. Icon Size. ( Defaults to 96 )
1. Background Transparency. ( Defaults to 1 )On.
1. 3dIcons Icon Set. ( Defaults to f).
   1. d = dynamic
   1. f = front
   1. i = iso
1. 3dIcons Icon Type. ( Defaults to c).
   1. m = clay
   1. c = color
   1. g = gradient
   1. p = premium
1. Icon List.
   1. A comma seperated list of short 3dIcon icon names to convert.

## Examples:
`3dIconify build/BASE.example`
Build a set of icons specified in the `build/BASE.example.3dicp` file.

`3dIconify build/3dIcons images - - - - pencil,explorer`
Build the pencil and explorer icons in images directory using app defaults.

# Related Software
[3dIcons](https://github.com/realvjy/3dicons) by
[@realvjy](https://github.com/realvjy)
