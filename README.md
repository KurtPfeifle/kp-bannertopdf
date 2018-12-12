# kp-bannertopdf
Quick'n'dirty shellscript-based hack to satisfy my need for a *'bannertopdf'* filter for the *'application/vnd.cups-banner'* format of CUPS on Linux

## Plan (for Work TBD)

1. ~~Write a ***sample banner text*** file (similar to *'vnd.cups-banner'* documented [here](https://www.cups.org/doc/spec-banner.html)) which shows the type of contents on the banner page we eventually want to support. Use *'vnd.kp-banner'* for now so not to conflict with other implementations. This will also serve as an initial rough spec for the format.~~   
**DONE**

1. ~~Write an auto-typing definition for this banner format in ***'kp-banner.types'*** to be placed in *'/usr/share/cups/banners/'*.~~   
**DONE**

1. ~~Write a ***'kp-bannertopdf'*** shell script to be placed in *'/usr/lib/cups/filters/'*. This script will evaluate whatever infos/requests are in the banner file and dynamically create a PDF page from this. The script will work in two stages:~~

    * ~~First create a Markdown (or HTML?) text file with the "dynamic" content.~~ **DONE**
    * ~~Then use an external program to convert the Markdown (the HTML) to PDF. (`'htmldoc'`?, `'pandoc'`?, `'enscript'`?, `'wkhtmltopdf'`?)~~ **DONE**
    * Optionally, use a(nother) external program to 'stamp' or 'background' some static content onto the PDF. (`'pdftk'` ?)

Let's start!

