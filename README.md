# Polytonic Extension

## Introduction

Polytonic Extension is a modified version of the STIX Two fonts, extended to support polytonic Greek.

The STIX Fonts project is ambitious, delivering a comprehensive set of fonts for publishing needs. The STIX Two fonts support the use of Greek in mathematics and other technical genres, as well as monotonic Greek text. Unfortunately, polytonic Greek is currently outside the scope of the project. Therefore, I have created this modified version simply to meet my needs.

My modified version uses the same source and build process as the original STIX fonts, and for the most part should inherit the same quality for Latin, Cyrillic and monotonic Greek. With regards to polytonic Greek, it lacks some features that you would expect from professional fonts.

The polytonic Greek glyphs are in Roman style only, the Italic style is not ready yet. However, Italic fonts are provided in the build, so that the *Italic* button will continue to work in word processors when typin in Latin, Cyrillic or monotonic Greek.

## STIX Two

The source STIX Two fonts are OpenType Unicode fonts for Scientific, Technical, and Mathematical texts, designed by Ross Mills, assisted by John Hudson and Paul Hanslow at Tiro Typeworks for the STI Pub companies.

Learn more about STIX Two:
* [https://www.tiro.com/fonts/stix-two](https://www.tiro.com/fonts/stix-two)
* [https://www.stixfonts.org/](https://www.stixfonts.org/)
* [https://github.com/stipub/stixfonts](https://github.com/stipub/stixfonts)

## Motivation

To meet the typography needs of a project I have been working on, after considering various options, I decided to modify STIX Two. My project involves translations and transliterations of texts in Church Slavonic and Koine Greek, and requires:
  * Latin, with diacritics
  * Polytonic Greek
  * Cyrillic, with a certain subset of Old Cyrillic characters and correctly placed diacritics

Preferably, these would have a unified appearance across all three scripts in a serif style including italics.

The only (Unicode) fonts that I have come across which correctly place diacritics on Cyrillic (where breathing and accent marks appear *side by side* above vowels like Greek, and the decimal *i* becomes *dotless* when accented) are from the [Ponomar Project](https://sci.ponomar.net/), but these are in historical style, which I want to avoid, and do not match Latin and Greek. I also tend to favour Greek fonts designed with horizontal stress. So I considered mainly the following options, and I decided that a modified version of STIX Two would seem to provide the most pleasing results with greatest flexibility.

* [Castoro](https://www.tiro.com/fonts/castoro), [SBL Greek](https://www.sbl-site.org/educational/BiblicalFonts_SBLGreek.aspx), and some other Cyrillic font (likely from Ponomar)

  SBL Greek is lighter than Castoro, and the companion Cyrillic would necessarily contrast.
* [Brill](https://www.tiro.com/fonts/brill)

  Looks like this would be ideal, however, version 4 lacks some Cyrillic and version 5 is not available for free non-commercial use.
* [Ladoga](https://www.myfonts.com/collections/ladoga-font-paratype)

  Has all the glyphs, but requires significant manual handling to correctly position and render accents and other glyphs.
* [STIX Two](https://www.tiro.com/fonts/stix-two)

  Has most glyphs, only a handful of additional glyphs need drawing, which the OFL licence allows.
* Other typefaces such as [Source Serif 4](https://adobe-fonts.github.io/source-serif/) and [Alegreya](https://huertatipografica.com/en/fonts/alegreya-ht-pro), which are similar in scope to STIX Two Text.

## This version

Polytonic Extension lacks features that would be expected from professional fonts, especially kerning, good hinting, and certain OpenType considerations (e.g. management of diacritics when uppercasing Greek, small caps). I use iota subscript everywhere, there is no provision for adscript. It is available in Regular, Medium, Semibold and Bold weights (and as a variable font), with no Italic style (Italic fonts are provided here so the *Italic* button will continue to work in Word processers when typing in Latin, Cyrillic or monotonic Greek, they are functionally no different to the official STIX Two Text fonts). I may alter the fonts from time to time without notice, for example if I decide outlines need tweaking or I want to improve kerning.

If STIX Two is ever updated to support polytonic Greek, [which is quite possible](https://github.com/stipub/stixfonts/issues/146), then my modified version will become obsolete.

The source can be found at [https://github.com/amoschou/stixfonts/tree/polytonic-extension-v2.14/extension](https://github.com/amoschou/stixfonts/tree/polytonic-extension-v2.14/extension).

## Copyright and license

```
Copyright 2001-2021 The STIX Fonts Project Authors (https://github.com/stipub/stixfonts), with Reserved Font Name "TM Math". STIX Fonts™ is a trademark of The Institute of Electrical and Electronics Engineers, Inc.

Additions for polytonic Greek © Andrew Moschou 2025.

This Font Software is licensed under the SIL Open Font License, Version 1.1.
```
