# Lǔbǐkè Zìtǐ

Lǔbǐkè Zìtǐ is derived from the Rubik Fonts. For more about the original version, please refer to [its project page](https://github.com/googlefonts/rubik).

## Introduction
As the default font of the wikifarm [Fandom](https://www.fandom.com/), Rubik supports the Latin, Cyrillic and Hebrew scripts. There are many non-Chinese Chinese-themed wikis on Fandom that need to display the Chinese Phonetic Alphabets, also known as *Hànyǔ Pīnyīn* or simply Pinyin, frequently. But unfortunately, Pinyin is not fully supported by Rubik font, which means the excluded alphabets will fallback to Arial or other fonts, causing inconsistency. Lǔbǐkè Zìtǐ (Lǔbǐkè is the Chinese phonetic spelling of Rubik, and zìtǐ means “font” in Chinese) is intended to solve the problem. Lǔbǐkè fully supports the commonly used Pinyin alphabets.

![Comparison before and after applying Lǔbǐkè Zìtǐ](https://github.com/Honoka55/lubike/blob/main/res/cmpr.png)

## Features
- All upper and lower case Pinyin alphabets that are already encoded in Unicode are supported, such as ǚ, ế and ǹ. The abbreviated forms specified in the Scheme for Chinese Phonetic Alphabet (*Hànyǔ Pīnyīn Fāng’àn*) are not included because no one actually uses them.
- This font is NOT designed for textbooks that teach Chinese as a foreign language. The *yángpíng* tone mark is still designed as an **acute** (wide at the top and narrow at the bottom), instead of following the Pinyin stroke order (wide at the bottom and narrow at the top).

## Usage
Try putting the following codes in your wiki’s Common.css. If it does’t work, download [the fonts](https://github.com/Honoka55/lubike/tree/main/fonts/ttf) and install them on your device.
``` css
@font-face {
    font-family: Lubike;
    src: url('https://cdn.jsdelivr.net/gh/Honoka55/lubike/fonts/ttf/Lubike-Regular.ttf');
}

@font-face {
    font-family: Lubike Italic;
    src: url('https://cdn.jsdelivr.net/gh/Honoka55/lubike/fonts/ttf/Lubike-Italic.ttf');
}

@font-face {
    font-family: Lubike Bold;
    src: url('https://cdn.jsdelivr.net/gh/Honoka55/lubike/fonts/ttf/Lubike-Bold.ttf');
}

@font-face {
    font-family: Lubike Bold Italic;
    src: url('https://cdn.jsdelivr.net/gh/Honoka55/lubike/fonts/ttf/Lubike-BoldItalic.ttf');
}

body.skin-fandomdesktop, button, input, textarea, .page-content :is(h2, h3, h4, h5, h6) .mw-headline, .fandom-community-header__community-name, h1#firstHeading {
	font-family: rubik,Lubike,helvetica,arial,sans-serif;
}
```
## License
Licensed under [the SIL Open Font License v1.1](https://github.com/Honoka55/QinglyuWuchenxian/blob/main/OFL.txt).

## Feedback
Issues and Pull Requests are welcome.
