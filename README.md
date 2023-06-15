## Obsidian Better PDF 2 Plugin

Goal of this Plugin in to implement a native PDF handling workflow in Obsidian
This version **2** was created as the original [Obsidian Better PDF Plugin](https://github.com/MSzturc/obsidian-better-pdf-plugin) was not updated anymore.

### Features

- Insert a single PDF Page inside Note
- Insert a list or range of pages into Obsidian Note
- Hyperlink to PDF
- Scale the size of PDF Pages to fit Note layout
- Rotate PDF
- Cutout PDF Parts

### Demo

![Sample](https://github.com/joleaf/obsidian-better-pdf-2-plugin/raw/master/sample/BetterPDF.gif)

### Syntax

as `json` string or `yaml`:

|parameter|required|example|
|--|--|--|
|url  |yes  |**myPDF.pdf** or **subfolder/myPDF.pdf** or "[[MyFile.pdf]]"
|link|optional (default = false)| **true** or **false**
|page|optional (default = 1)| **1** or **[1, [3, 6], 8]** where **[3, 6]** is an inclusive range of pages. page = 0 is an alias for the whole document
|range|optional| **[1, 3]** Insert pages **1** to **3** (inclusive). Overwrites page.
|scale|optional (default = 1.0)| **0.5** for 50% size or **2.0** for 200% size
|fit|optional (default = true)| **true** or **false**
|rotation|optional (default = 0)| **90** for 90deg or **-90** -90deg or **180**
|rect|optional (default = \[0,0,0,0\])| offsetX, offsetY, sizeY, sizeX in Pixel

#### Example json (from the original Better PDF plugin)
````
```pdf
{
  "url" : "[[My_pdf.pdf]]",
  "page": 1
}
```
````

#### Example yaml (new syntax)
````
```pdf
url: [[My_pdf.pdf]]
page: 1
```
````


### Integration
- [JavaScript for Adobe Acrobat Pro and AppleScript for Skim for creating automatically the necessary Better PDF Plugin snippet](https://github.com/johnsidi/scripts-for-Obsidian-Better-PDF-Plugin)

## Donate

<a href='https://ko-fi.com/joleaf' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />