# Fonts 🕹️

Monospace fonts are better optimized for code readability and alignment. Here is a list of awesome coding fonts that I've used in the past. But I always come back to `Fira Code`.
## List of Awesome Fonts

### Free Fonts

1. [Fira Code](https://github.com/tonsky/FiraCode)
2. [Hack](https://github.com/source-foundry/Hack)
3. [Monoid](https://github.com/larsenwork/monoid)
4. [Hasklig](https://github.com/i-tu/Hasklig)
5. [Input Mono](https://github.com/powerline/fonts/tree/master/InputMono)
6. [Office Code Pro](https://github.com/nathco/Office-Code-Pro)
7. [Inconsolata](https://github.com/googlefonts/Inconsolata)
8. [DejaVu Sans Mono](https://github.com/dejavu-fonts/dejavu-fonts)
9. [Droid Sans Mono](https://github.com/chrissimpkins/codeface/tree/master/fonts/droid-sans-mono)
10. [Source Code Pro](https://github.com/adobe-fonts/source-code-pro)

### Paid Fonts

1. [Operator Mono](https://www.typography.com/fonts/operator/styles/)
2. [Dank Mono](https://dank.sh/)
3. [PragmataPro](https://www.fsd.it/shop/fonts/pragmatapro/)

## Installing Fonts

### On Ubuntu

Even on same OS, installation procedure can vary between different fonts. On ubuntu, `open type` fonts generally live in `/usr/share/fonts/opentype/` folder.

* To install `Fira Code` you can simply type:
    ```bash
    $ sudo apt install fonts-firacode
    ```

* However, this often downloads older version of the font. Recently they released a sleeker version 2.0 of the font. To install that, download the font from [here.](https://github.com/tonsky/FiraCode/releases/download/2/FiraCode_2.zip). Unzip the font folder and go to `otf` folder. Then simply run:

    ```bash
    $ sudo cp -a . /usr/share/fonts/opentype/firacode
    ```
