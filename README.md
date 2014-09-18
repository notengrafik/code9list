# code9list

PostScript program that renders a graphical listing of Score's DRW files.

##Usage

This program requires Ghostscript to be installed.  [Download code9list.ps](https://github.com/th-we/code9list/blob/master/code9list.ps) to your Score LIB directory.

###Linux/Mac

* Open a terminal at your Score LIB directory
* To create a PDF listing, type:<br/>
  `gs -sDEVICE=pdfwrite -o code9list.pdf code9list.ps`

### Windows

* Open a command prompt at your Score LIB directory
* Find out where your Ghostscript executable is stored (`gswin32c.exe` or `gswin64c.exe`)
* Assuming Ghostscript is fount at `C:\Program files\gs\bin\gswin64c.exe`, to create a PDF listing, type:<br/>
  `C:\Program files\gs\bin\gswin64c.exe -sDEVICE=pdfwrite -o code9list.pdf code9list.ps`

## Notes

As the scale of Code 9 symbols varies, all symbols are scaled to the maximum size that fits inside a box of the listing.  This means, items will be displayed out of scale relative to each other.
