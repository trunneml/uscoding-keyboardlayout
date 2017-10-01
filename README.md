# Improved Version Of The US International Keyboard Layout

> US International Keyboard Layout without dead keys on stupid positions.

This Windows keyboard layout is based on the Microsoft US International keyboard layout. On the original layout ' and \` are dead keys. So characters often needed while coding, needed multiple key presses. Because of that most software developers are switching between standard US keyboard layout for programming and their native language keyboard layout for writing emails.

US Coding just moved the dead keys of the US International keyboard layout to the AltGr layer. This way it feels like the normal US keyboard layout, but with the full character support of the international version and no keyboard layout switching is needed to write a email in French or German.

This layout (including the `setup.exe`) was created using the [Microsoft Keyboard Layout Creator 1.4](https://www.microsoft.com/en-us/download/details.aspx?id=22339).

**Compatibility**: Windows 7, 8, 8.1 and Windows 10; including 32Bit & 64Bit (amd64 & ia64) versions.

## Layers and Differences to the original US International Keyboard Layout
- Restored ^, \` and ~.
- Dead Keys ^, \` and ~ moved to the AltGr Layer.
- ¼, ½, ¾ moved to the Shift + AltGr Layer.
- Dead keys followed by a `Space` will create a **UTF-8 combining character**.


### Comparison

| Character | US-Coding          | US-Standard  | US-International      |
| :-------: | ------------------ | ------------ | --------------------- |
| `         | `                  | `            | ` , **Space**         |
| ~         | Shift + `          | Shift + `    | Shift + `, **Space**  |
| '         | '                  | '            | ' , **Space**         |
| "         | Shift + '          | Shift + '    | Shift + ' , **Space** |
| ^         | Shift + 6          | Shift + 6    | Shift + 6 , **Space** |
| ¼         | Shift + AltGr + 6  | *Impossible* | AltGr + 6             |
| Ä         | AltGr + Shift + q  | *Impossible* | AltGr + Shift + q     |
| ß         | AltGr + s          | *Impossible* | AltGr + s             |
| €         | AltGr + 5          | *Impossible* | AltGr + 5             |
| è         | AltGr + `, e       | *Impossible* | `, e                  |
| ý         | AltGr + ', y       | *Impossible* | ', y                  |


### Combining Character

In digital typography, combining characters are characters that are intended to modify other characters. 

| Character | Unicode                                                               | Key Sequence      | Example |
| :-------: | --------------------------------------------------------------------- | ----------------- | :-----: |
|    ̀       | [U+0300](http://www.fileformat.info/info/unicode/char/0300/index.htm) | AltGr + `, Space  |    à    |
|    ́       | [U+0301](http://www.fileformat.info/info/unicode/char/0301/index.htm) | AltGr + ', Space  |    á    |
|    ̂       | [U+0302](http://www.fileformat.info/info/unicode/char/0302/index.htm) | AltGr + 6         |    â    |
|    ̃       | [U+0303](http://www.fileformat.info/info/unicode/char/0303/index.htm) | AltGr + ~, Space  |    ã    |
|    ̈       | [U+0308](http://www.fileformat.info/info/unicode/char/0308/index.htm) | AltGr + Shift + ' |    ä    |

It's possible to stack multiple combining characters: ý̀ c̈̃

For more information see: https://en.wikipedia.org/wiki/Combining_character

### Layers in detail

#### Base Layer
![Base Layer](images/USCoding.jpg)

#### Shifted Base Layer
![Shifted Base Layer](images/USCodingShft.jpg)

#### AltGr Layer
![AltGr Layer](images/USCodingAltGr.jpg)

#### Shifted AltGr Layer
![Shifted AltGr Layer](images/USCodingShftAltGr.jpg)


## Installation
Just download the [latest release](https://github.com/trunneml/uscoding-keyboardlayout/releases/latest), unzip it and run `setup.exe`.


## Manual Build

1. Download and install [Microsoft Keyboard Layout Creator 1.4](https://www.microsoft.com/en-us/download/details.aspx?id=22339)
2. Open the `uscoding.klc` file
3. Project -> Build DLL and Setup Package
4. *(Optional)* Zip the created files