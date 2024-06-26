# Steganography Data Extractor

This script allows you to extract general information and hidden data 
from image files using steganography tools.

## Prerequisites

The script will automatically check for the required steganography tools
and install them if they are missing. You do not need to manually install them.

- [Steghide](http://steghide.sourceforge.net/)
- [Outguess](https://github.com/outguess/outguess)
- [Stegseek](https://github.com/RickdeJager/stegseek)
- [Binwalk](https://github.com/ReFirmLabs/binwal)
- [Exiftool](https://github.com/exiftool/exiftool)

#### NOTE:

This tool was developed and tested on a Debian distribution of Linux.
Tools will be automatically installed if the environment is a Debian distro.

## Usage

```
./stegtool.sh <image_file> [password] [wordlist.txt]
```

<image_file>: Path to the image file from which data will be extracted.<br>
[password]: Optional password for extracting embedded files.<br>
[wordlist.txt]: Optional wordlist file for extracting embedded files using stegseek. Required only when using stegseek.<br>

## Examples

```
./stegtool.sh image.jpg '' wordlist.txt
```

## License

The code in this project is licensed under MIT license.
