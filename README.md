# Noto CJK Subset Webfonts

Noto CJK subset web fonts are based on [Noto Serif CJK Version 2.003](https://github.com/notofonts/noto-cjk/releases/tag/Serif2.003).

- [Noto CJK Subset Webfonts](#noto-cjk-subset-webfonts)
  - [Github](#github)
  - [Directure Structure](#directure-structure)
  - [Overview](#overview)
  - [Install](#install)
  - [Usage](#usage)
    - [Simplified Chinese](#simplified-chinese)
    - [Traditional Chinese](#traditional-chinese)
    - [Japanese](#japanese)
    - [Korean](#korean)
  - [License](#license)

## Github

<https://github.com/w3labkr/noto-cjk>

## Directure Structure

```txt
.
|-- subset/
|   `-- <font-family>/
|       `-- <character-set>/
|-- LICENSE
`-- README.md
```

## Overview

Glyphs

```txt
| Font-family | Character set | Glyphs |
|-------------|---------------|--------|
| NotoSansKR  | slim          | 3,985  |
| NotoSansKR  | standard      | 8,547  |
| NotoSansJP  | standard      | 7,213  |
| NotoSansSC  | slim          | 4,322  |
| NotoSansSC  | standard      | 7,590  |
| NotoSansTC  | slim          | 4,673  |
| NotoSansTC  | standard      | 13,998 |
```

CSS font-face property

```css
@font-face {
  font-weight: 100..900;
  font-family: "Noto {Sans, Serif} {KR, JP, SC, TC}";
  font-style: normal;
  src: url("FontFamily-FontWeight.woff2") format("woff2"), url("FontFamily-FontWeight.woff") format("woff");
}
```

CSS font-weight property

```txt
| font-weight | NotoSans   | NotoSerif  |
|-------------|------------|------------|
| 100         | Thin       | -          |
| 200         | ExtraLight | ExtraLight |
| 300         | Light      | Light      |
| 400         | Regular    | Regular    |
| 500         | Medium     | Medium     |
| 600         | SemiBold   | SemiBold   |
| 700         | Bold       | Bold       |
| 800         | ExtraBold  | ExtraBold  |
| 900         | Black      | Black      |
```

## Install

html

```html
<link rel="stylesheet" href="font.css" />
```

stylesheet

```css
@import url('font.css');
```

cdn

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/<font-family>/<character-set>/font.min.css" crossorigin="anonymous" />
```

## Usage

### Simplified Chinese

Simplified Chinese characters are standardized Chinese characters prescribed in the Table of General Standard Chinese Characters for use in *mainland China*.

Sans-serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansSC/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansSC/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Sans SC', sans-serif; }
```

Serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifSC/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifSC/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Serif SC', serif; }
```

### Traditional Chinese

Traditional Chinese characters are currently used in *Hong Kong*, *Macau*, and *the Republic of China (Taiwan)*.

Sans-serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansTC/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansTC/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Sans TC', sans-serif; }
```

Serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifTC/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifTC/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Serif TC', serif; }
```

### Japanese

Sans-serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansJP/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Sans JP', sans-serif; }
```

Serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifJP/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Serif JP', serif; }
```

### Korean

Sans-serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansKR/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSansKR/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Sans KR', sans-serif; }
```

Serif

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifKR/slim/font.min.css" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/w3labkr/noto-cjk/subset/NotoSerifKR/standard/font.min.css" crossorigin="anonymous" />
```

```css
body { font-family: 'Noto Serif KR', serif; }
```

## License

Noto CJK subset web fonts are licensed under the [SIL Open Font License, Version 1.1.](LICENSE)
