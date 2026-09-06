# Chrysanthemum

## 项目简介 / INTRODUCTION

Chrysanthemum 是一款以 SIL OFL 1.1 协议开源的西文衬线字体，包括正体和斜体，目前仅有一个字重。

## 项目结构 / STRUCTURE

```text
.
├── Source
│        ├── c.fcp                         # 正体源文件
│        └── c-Italic.fcp                  # 斜体源文件
├── WOFF
│      ├── Chrysanthemum-Italic.woff
│      ├── Chrysanthemum-Italic.woff2
│      ├── Chrysanthemum-Regular.woff
│      └── Chrysanthemum-Regular.woff2
├── Chrysanthemum-Italic.otf
├── Chrysanthemum-Regular.otf
├── LICENSE                                # SIL Open Font License 1.1
├── OFL-FAQ.txt
├── README.md                              # 本文件
└── FontCreator_Badge_01.png               # Made With FontCreator 15.0!
```

## 许可证 / LICENSE

- 本字体以 [SIL Open Font License](https://openfontlicense.org/open-font-license-official-text/) 1.1 发布。

- 你可以自由分享、修改本字体，但必须保留原有的全部版权声明，且不得使用保留名称（Reserved Font Name），且衍生作品需以相同许可证分发。

## 致谢 / ACKNOWLEDGEMENTS

- 正体大部分字母与符号、斜体大写字母、旧体数字：衍生自 [Theano Old Style](https://www.1001fonts.com/theano-old-style-font.html)。

- 斜体小写字母：衍生自 [Libre Baskerville](https://github.com/impallari/Libre-Baskerville)  [（或1001 Fonts链接）](https://www.1001fonts.com/libre-baskerville-font.html)。

- 等宽、比例阿拉伯数字：衍生自 [BIZ UDPMincho](https://fonts.adobe.com/fonts/biz-udpmincho)  [（或いいフォント/goodfreefonts链接）](https://goodfreefonts.com/456/)。

- 修改字体使用软件：FontCreator 15.0.0.2927

![Made With FontCreator 15.0](FontCreator_Badge_01.png "FontCreator")

## 彩蛋1：为什么版本号是 1.310？

- 1.000：一个比较粗糙的版本，数字的高度与字母不协调。

- 1.100：修正了数字的高度，并在私用区中添加了等宽数字的字形（但未加入 `tnum` 特性）。

    在 1.000 版本中，斜体的某些字符是正体生硬倾斜得到的（实际上不该如此）。1.1.000版本修复了这个问题。

    修正了斜体某些字符倾斜度过大的问题。

- 1.200：加入了 `tnum` 特性。

    修改了斜体部分小写字母的前后空白和部分 kerning 值。

- 1.300：等宽数字宽度不变，而字形变窄，使得两侧负空间更大，解决了某些数字组合间距过小而不够美观的问题。

    调高了字符“¤”（`U+00A4`，货币符号，Currency Sign）的高度。

- 1.310：比例数字 1 与 0、0 与 0、0 与 1之间加入负值的 kerning（人话：间距减小了），进一步使数字间距协调。

## 彩蛋2：Chrysanthemum 的名称来源？
-   这个名字几乎就是随便取的，没有什么特殊的寓意。

    根据 OFL 协议的规定，衍生字体不得使用源字体的保留名称。我选择了这个意为“菊花”的英文单词作为新字体的名称。

## 彩蛋3：关于等宽数字
- 在 FontCreator 中，可以看见本字体“每格宽度”是2048，而等宽数字的宽度是 1024，恰好是 2048 的一半。也就是说，若尝试用该字体和常见中文字体进行中西混合排版，用该字体排版西文和数字，并开启该字体的 `tnum` 特性，会发现数字的宽度恰好是汉字宽度的一半。这是为了在中文排版中让数字和汉字有较好的兼容性。

    题外话 1：实际上，Windows 系统的默认中文字体“宋体（SimSun）”“黑体（SimHei）”等等的数字和西文字符的宽度都是汉字的一半。不过 Windows 系统默认的中文字体自带的西文部分字形较丑陋。

    题外话 2：日文字体 MS PMincho 的西文字符比大多数为中日韩文字设计的字体自带的西文字符美观得多，因为 MS PMincho 的西文字符是比例宽度，不是等宽的。
