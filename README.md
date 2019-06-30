# An analysis of the behaviour of the digital rain in The Matrix

The purpose of this document is to share an understanding of the behaviour and appearance of the iconic digital rain visual effect used in The Matrix. This can be used to provide a guide of sorts when attempting to emulate the effect.

This document is a work in progress:

- [x] Animation
    - [x] Falling code
    - [x] Changing glyphs
    - [x] Deletion strings
    - [x] Highlighted glyphs
- [ ] Composition
    - [ ] Grid
    - [x] Glyphs used
    - [ ] Typeface
    - [ ] Colours

The sample used for study is that in the opening sequence of the first movie.

![The opening sequence, The Matrix, 1999](img/01.gif)

This analysis does not include other samples for the following reasons:

* The digital rain behaves differently in the sequels
* This is the clearest and most iconic example of the effect

## Glossary

* **Digital rain** or **code**: The overall visual effect used to demonstrate the underlying code of The Matrix
* **Glyph**: A single text character
* **String**: An unbroken set of glyphs in a single column
* **Frame**: A single moment of the animation

## Animation

### Falling code

At first glance the glyphs appear to move down from the top to the bottom of the screen, however, the first thing to notice when isolating a single string is that the glyphs themselves do not descend:

![Glyphs that remain in place](img/02.gif)

Except for changing glyphs, they remain in place, and different glyphs appear beneath them.

Additionally, it appears that the strings don't always originate from the top of the screen:

![Glyphs that appear lower down the screen](img/03.gif)

It looks as though new strings are being created at points lower down the screen. However, the pauses in time between these strings appearing suggest that invisible characters exist. For instance, if we were to insert a placeholder character in locations which we predict a character for that frame, we can see the pattern:

![Evidence of invisible characters](img/04.gif)

We can therefore assume that the first of the visible glyphs in this string did not spawn in the middle of the screen, but was also preceded by invisible characters.

### Changing glyphs

Some glyphs remain static for three frames, and then change into another glyph:

![Changing glyph](img/05.gif)

During a single frame, the new and old glyph occupy the same space, each at 50% opacity. All changing glyphs change on the same frame. Some strings consist entirely of changing glyphs.

### Deletion strings

Deletion strings only generate invisible characters. Unlike regular strings, deletion strings can appear over the top of existing strings. While we cannot see the deletion string itself, we can see evidence of it when an existing string disappears:

![Evidence of deletion strings](img/06.gif)

### Highlighted glyphs

Roughly 1 in 5 strings have highlighted glyphs. Only a single glyph of a string is highlighted at a given time, and that glyph is leading glyph of the string:

![Evidence of highlighted glyphs](img/07.gif)

The only exception to the above rule of only a single glyph of a string being highlighted at a given time, is that every so often, all highlighted glyphs will stammer at the same time. The stammer causes strings with highlighted glyphs to fall behind other strings by a single row:

![Highlight glyph stammering](img/08.gif)

| Frame  | Leading glyph            | Second to leading glyph | String length |
| ------ | ------------------------ | ----------------------- | ------------- |
| 0      | Highlighted              | Normal                  | 1             |
| 1      | Partially highlighted    | Partially highlighted   | 2             |
| 2      | Highlighted              | Normal                  | 2             |
| 3      | Highlighted              | Normal                  | 3             |

## Composition

### Glyphs used

#### Kangxi radical

| Glyph | Name          | Screenshot                           |
| ----- |-------------- | ------------------------------------ |
| `日`  | Han character | ![Han character](img/kangxi-han.gif) |

#### Katakana

These glyphs are flipped horizontally.

| Glyph | Name         | Screenshot                            |
| ----- | ------------ | ------------------------------------- |
| `ﾊ`   | ha syllable  | ![ha syllable](img/katakana-ha.gif)   |
| `ﾋ`   | hi syllable  | ![hi syllable](img/katakana-hi.gif)   |
| `ｼ`   | shi syllable | ![shi syllable](img/katakana-shi.gif) |
| `ﾂ`   | tsu syllable | ![tsu syllable](img/katakana-tsu.gif) |
| `ｳ`   | u syllable   | ![u syllable](img/katakana-u.gif)     |
| `ｰ`   | long-vowel   | ![long-vowel](img/katakana-lv.gif)    |
| `ﾅ`   | na syllable  | ![na syllable](img/katakana-na.gif)   |
| `ﾐ`   | mi syllable  | ![mi syllable](img/katakana-mi.gif)   |
| `ﾓ`   | mo syllable  | ![mo syllable](img/katakana-mo.gif)   |
| `ﾆ`   | ni syllable  | ![ni syllable](img/katakana-ni.gif)   |
| `ｻ`   | sa syllable  | ![sa syllable](img/katakana-sa.gif)   |
| `ﾜ`   | wa syllable  | ![wa syllable](img/katakana-wa.gif)   |
| `ｵ`   | o syllable   | ![o syllable](img/katakana-o.gif)     |
| `ﾘ`   | ri syllable  | ![ri syllable](img/katakana-ri.gif)   |
| `ﾎ`   | ho syllable  | ![ho syllable](img/katakana-ho.gif)   |
| `ﾏ`   | ma syllable  | ![ma syllable](img/katakana-ma.gif)   |
| `ｴ`   | e syllable   | ![e syllable](img/katakana-e.gif)     |
| `ｷ`   | ki syllable  | ![ki syllable](img/katakana-ki.gif)   |
| `ﾑ`   | mu syllable  | ![mu syllable](img/katakana-mu.gif)   |
| `ﾃ`   | te syllable  | ![te syllable](img/katakana-te.gif)   |
| `ｹ`   | ke syllable  | ![ke syllable](img/katakana-ke.gif)   |
| `ﾒ`   | me syllable  | ![me syllable](img/katakana-me.gif)   |
| `ｶ`   | ka syllable  | ![ka syllable](img/katakana-ka.gif)   |
| `ﾕ`   | yu syllable  | ![yu syllable](img/katakana-yu.gif)   |
| `ﾗ`   | ra syllable  | ![ra syllable](img/katakana-ra.gif)   |
| `ｾ`   | se syllable  | ![se syllable](img/katakana-se.gif)   |
| `ﾈ`   | ne syllable  | ![ne syllable](img/katakana-ne.gif)   |
| `ｽ`   | su syllable  | ![su syllable](img/katakana-su.gif)   |
| `ﾀ`   | ta syllable  | ![ta syllable](img/katakana-ta.gif)   |
| `ﾇ`   | nu syllable  | ![nu syllable](img/katakana-nu.gif)   |

#### Arabic numerals

There doesn't appear to be separate characters for `6` and `9`. They either share the same character or one is missing.

| Numeral | Screenshot             | Transformation       |
| ------- | ---------------------- | -------------------- |
| `0`     | ![0](img/arabic-0.gif) | None                 |
| `1`     | ![1](img/arabic-1.gif) | None                 |
| `2`     | ![2](img/arabic-2.gif) | Flipped horizontally |
| `3`     | ![3](img/arabic-3.gif) | Flipped vertically   |
| `4`     | ![4](img/arabic-4.gif) | None                 |
| `5`     | ![5](img/arabic-5.gif) | Flipped horizontally |
| `6`     | ![6](img/arabic-6.gif) | Flipped vertically   |
| `7`     | ![7](img/arabic-7.gif) | None                 |
| `8`     | ![8](img/arabic-8.gif) | None                 |
| `9`     | ![9](img/arabic-6.gif) | Flipped horizontally |

#### English alphabet

| Glyph | Screenshot              |
| ----- | ----------------------- |
| `Z`   | ![Z](img/english-z.gif) |

#### Other

| Glyph | Name             | Screenshot                                |
| ----- | ---------------- | ----------------------------------------- |
| `*`   | asterisk         | ![asterisk](img/asterisk.gif)             |
| `+`   | plus             | ![plus](img/plus.gif)                     |
| `:`   | colon            | ![colon](img/colon.gif)                   |
| `=`   | equals           | ![equals](img/equals.gif)                 |
| `.`   | period           | ![period](img/period.gif)                 |
| `<`   | less-than        | ![less-than](img/less-than.gif)           |
| `>`   | more-than        | ![more-than](img/more-than.gif)           |
| `"`   | double quotation | ![double quotation](img/double-quote.gif) |
| `｜`  | vertical bar     | ![vertical bar](img/vertical-bar.gif)     |
| `¦`   | broken bar       | ![broken bar](img/broken-bar.gif)         |
| `_`   | underscore       | ![underscore](img/underscore.gif)         |