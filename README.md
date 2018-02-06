R Markdown quickstart
================
Foon Wong
January 31, 2018

-   [Introduction](#introduction)
-   [Quick start](#quick-start)
-   [Resources and links](#resources-and-links)
-   [pdf documents](#pdf-documents)
-   [LaTeX Math](#latex-math)
-   [Practical Tips](#practical-tips)
-   [Useful hotkeys](#useful-hotkeys)
-   [Where to get help](#where-to-get-help)

#### Introduction

Rmarkdown is a wonderful way to generate high quality reports for all your R projects. Here's some resources and tips to help you get started.

#### Quick start

-   Follow the wizard to create a new document.
    <img src="newfile.png" width="250" />

-   The default new file explains the structure.

1.  *YAML header* in which you can specify your document metadata, output [formats](http://rmarkdown.rstudio.com/formats.html) and other global options.

2.  [Text](http://www.stat.cmu.edu/~cshalizi/rmarkdown/#basic-formatting-in-r-markdown) written in markdown, which will be automatically converted into other formats: html, pdf, word documents and etc. The syntax is simple and you can learn all the basics in 5 minutes.

3.  [R code chunks](http://www.stat.cmu.edu/~cshalizi/rmarkdown/#including-code) (**Ctrl + Alt + I **) R code can be easily inserted inline, or written in chunks. All code written in the chunks are executed when you knit the file. By default, both the code and output is displayed.

<img src="default.png" width="600" />

-   Hit **Ctrl + Alt + K** to knit or render your document. Easy!

#### Resources and links

-   [Using R Markdown for Class Reports](http://www.stat.cmu.edu/~cshalizi/rmarkdown/): Fantastic guide by Cosma Shalizi. Must read. I am referencing it as I am writing this now.

-   [Official introduction](http://rmarkdown.rstudio.com/lesson-1.html): If you are totally foreign to rmarkdown. Check out Rstudio's great tutorial and examples.

-   [Official cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/rmarkdown-2.0.pdf)

-   [Markdown live preview](http://markdownlivepreview.com/): A quick way to understand how to write markdown if you have never written markdown before. See instantaneously how the markdown syntax works. It's also a great tool for troubleshooting.

-   [ShareLaTeX](https://www.sharelatex.com/): While rstudio does preview for LaTeX math, it's really better to edit LaTeX code with purpose built tools.

-   [KableExtra](https://haozhu233.github.io/kableExtra/): awesome styling options for your tables.

#### pdf documents

pdf documents are typesetted using LaTeX. Installation links:
- [MikTex](https://miktex.org/download) (Windows) Download the "net installer" and choose complete installation (Large file!).

-   [MacTex](https://tug.org/mactex/mactex-download.html) (Mac).

-   If you need to use LaTeX packages, modify your YAML like so:

<!-- -->

    ---
    title: 'Homework I (Part II)'
    author: "Foon Wong"
    date: "February 4, 2018"
    output: pdf_document
    header-includes:
    - \usepackage{amsmath}
    - \usepackage{amssymb}
    ---

#### LaTeX Math

Rmarkdown has support for a lot of LaTeX commands. Just like a regular TeX document, you can have:
- inline math: surround your LaTeX code with a pair of `$`.
- Longer blocks of math: write between `\[` and `\]`.

#### Practical Tips

-   Organize your document using headers. The character `#` means the rest of the line is interpreted as a header. This allows you to quickly jump to (**Shift + Alt + J**) and hide (**Alt + O**) different sections of your document.

<img src="navigation.png" width="400" />

-   Name your code chunks. Facilitates navigation and troubleshooting.

-   Use the packages kable and kableExtra to format your tables. It can do some really cool things in html.

-   Starting a new line. Don't forget to end your line with two spaces.

-   LaTeX Math: LaTeX rendering can be very sensitive to spacing. If you have newlines in between \`$'s, it may break.

#### Useful hotkeys

**Ctrl + Shift + K**: knits the text file to your desired output format.
**Ctrl + Alt + I (OS X: Cmd + Option + I)**: Inserts a r code chunk.
**Ctrl + Shift + Enter**: Execute a code chunk.
**Shift + Alt + J**: Navigation.

#### Where to get help

[StackOverflow](https://stackoverflow.com/)
