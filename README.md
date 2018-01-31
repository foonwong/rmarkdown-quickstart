R Markdown quickstart
================
Foon Wong
January 31, 2018

### Introduction

Rmarkdown is a wonderful way to generate high quality reports for all your R projects.

There are many great resources on the web. In this document, you will find links to those resources and helpful tips to get started.

### Motivation

This page you are seeing was created using knitr() built in to the lastest Rstudio. This is an example of a special markdown document that display nciely on GitHub. This is a great way of sharing information without hosting your own site.

You can also create interactive pages in html.

In addition, you can create beautifully typesetted documents without learning LaTeX.

### Structure

A R markdown document consists of the following components:
1. *YAML header* in which you can specify your document metadata and output format.

1.  *Text* written in markdown, which can be easily converted into other formats: html, pdf, word documents and etc. The syntax is simple and you can learn all the basics in 5 minutes.

2.  *R code chunks* and output. You have great control on how your code is formatted in between your text.

### Resources and links

-   [Official introduction](http://rmarkdown.rstudio.com/lesson-1.html): Rstudio has great tutorial and examples. See what it can do!

-   [Official cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/rmarkdown-2.0.pdf)

-   [Markdown live preview](http://markdownlivepreview.com/): there's no better way of learning than by experimenting. See instantaneously how the markdown syntax works.

### Useful hotkeys (windows)

**Ctrl + Shift + K**: knits the text file to your desired output format. **Ctrl + Alt + I**: Inserts a r code chunk.

### Software depedencies

#### pdf documents

-   [MikTex](https://miktex.org/download). Windows. Download the "net installer" and choose complete installation (Large file!).

### Where to get help

### Beginner tips

-   R markdown does not insert a line break even if you have a new line on your text file. If you want a line break, you must type two spaces at the end of the line.
