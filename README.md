# jupyterthemes
## Theme-ify your Jupyter Notebooks!

```sh
jt -t chesterish -cw 850 -f hack -fs 10
```
![image](https://github.com/dunovank/jupyter-themes/blob/master/screens/jt-tchesterish-cw850-fs10.png?raw=true)

```sh
jt -t oceans16 -alt -f hack -fs 10 -cw 900
```
![image](https://github.com/dunovank/jupyter-themes/blob/master/screens/jt-toceans16-altmd-fs10-cw900.png?raw=true)

```sh
jt -t onedork -f hack -fs 10 -cw 850
```
![image](https://github.com/dunovank/jupyter-themes/blob/master/screens/jt-tonedork-cw850-fs10.png?raw=true)

```sh
jt -t grade3 -alt -fs 10 -cw 900 -tf ptserif
```
![image](https://github.com/dunovank/jupyter-themes/blob/master/screens/jt-tgrade3-altmd-fs10-cw900.png?raw=true)

```sh
jt -t onedork -nf ptserif -tf ptserif
```
![image](https://github.com/dunovank/jupyter-themes/blob/master/screens/jt-tonedork-ffserif-tcffserif.png?raw=true)

# Install with pip
```sh
pip install jupyterthemes
```

## Command Line Usage

```
usage: jt [-h] [-l] [-t THEME] [-f MONOFONT] [-fs MONOSIZE] [-nf NBFONT]
          [-nfs NBFONTSIZE] [-tf TCFONT] [-tfs TCFONTSIZE] [-cw CELLWIDTH]
          [-lh LINEHEIGHT] [-alt] [-vim] [-T] [-N] [-r]
```

|        options        |   arg     |     default    |
|:----------------------|:---------:|:--------------:|
| Usage help            |  -h       |       --       |
| List Themes           |  -l       |       --       |
| Theme Name to Install |  -t       |       --       |
| Code Font             |  -f       |     source     |
| Code Font-Size        |  -fs      |       11       |
| NB Font               |  -nf      |    opensans    |
| NB Font Size          |  -nfs     |       13       |
| Txt and MD Font       |  -tf      |     ptserif    |
| Txt and MD Fontsize   |  -tfs     |       13       |
| Cell Width            |  -cw      |      980       |
| Line Height           |  -lh      |      170       |
| Alt Txt/MD Layout     |  -alt     |       --       |
| Style Vim NBExt       |  -vim     |       --       |
| Toolbar Visible       |  -T       |       --       |
| Name & Logo Visible   |  -N       |       --       |
| Restore Default       |  -r       |       --       |


## Examples
```sh
# list available themes
# oceans16 | grade3 | chesterish | onedork
jt -l

# select theme...
jt -t chesterish

# toggle toolbar ON and notebook name ON
jt -t grade3 -T -N

# set code font to 'Roboto Mono' 12pt
# (see monospace font table below)
jt -t oceans16 -f roboto -fs 12

# set code font to Fira Mono, 11.5pt
# 3digit font sizes converted into floats (115-->11.5pt)
jt -t grade3 -f fira -fs 115

# set notebook & text-cell fonts
# (see sans-serif & serif font tables below)
jt -t onedork -nf ptserif -tf droidsans

# adjust cell width and line-height
jt -t chesterish -cw 900 -lh 170

# choose alternate txt/markdown layout
jt -t grade3 -alt

# restore default theme
jt -r
```

## Monospace Fonts (codecells)
| -f arg | Monospace Font |
|:--|:--|
|anka|Anka/Coder|
|anonymous|Anonymous Pro|
|aurulent|Aurulent Sans Mono|
|bitstream|Bitstream Vera Sans Mono|
|bpmono|BPmono|
|code|Code New Roman|
|consolamono|Consolamono|
|cousine|Cousine|
|dejavu|DejaVu Sans Mono|
|droidmono|Droid Sans Mono|
|fira|Fira Mono|
|firacode|Fira Code|
|generic|Generic Mono|
|hack|Hack|
|inconsolata|Inconsolata-g|
|liberation|Liberation Mono|
|meslo|Meslo|
|office|Office Code Pro|
|oxygen|Oxygen Mono|
|roboto|Roboto Mono|
|saxmono|saxMono|
|source|Source Code Pro|
|sourcemed|Source Code Pro Medium|
|ubuntu|Ubuntu Mono|

## Sans-Serif Fonts
| -nf/-tf arg | Sans-Serif Font |
|:--|:--|
|droidsans|Droid Sans|
|latosans|Lato|
|opensans|Open Sans|
|ptsans|PT Sans|
|robotosans|Roboto|
|sourcesans|Source Sans Pro|

## Serif Fonts
| -nf/-tf arg | Serif Font |
|:--|:--|
|crimsonserif|Crimson Text|
|droidserif|Droid Serif|
|ebserif|EB Garamond|
|loraserif|Lora|
|merriserif|Merriweather|
|ptserif|PT Serif|
