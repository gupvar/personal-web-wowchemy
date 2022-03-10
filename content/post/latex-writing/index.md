---
title: Speed-writing Tools for LaTeX
subtitle: Get started using LaTex in no time.

# Summary for listings and search engines
summary: Get started using LaTex in no time.

# Link this post with a project
projects: []

# Date published
date: "2020-12-13T00:00:00Z"

# Date updated
lastmod: "2020-12-13T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/05A-kdOH6Hw)'
  focal_point: ""
  placement: 1
  preview_only: false

authors:
- admin

tags:
- Academic
- Writing
- LaTeX

categories:
- Research
---

## What is LaTeX?

Most of my professional writing – including papers, class presentation slides, assignments are made in LaTeX (pronounced «Lah-tech» or «Lay-tech» ). LaTeX is a markup (programming) language that is different from typesetting tools such as MS-Word or MS-PowerPoint where you see immediately what you write and also take care of formatting at the same time. The utmost power of https://miktex.org/LaTeX comes with the precision and its ability to control the formatting for documents including alignment, sectioning, auto-referencing, and for me its ability to easily render (near-)perfect mathematical writing.

## Getting started with LaTeX

In order to use LaTeX on your computer, you will need to install the basic libraries (MikTex: https://miktex.org/) and a front-end text editor (I use Texmaker). There are many front-end editors such as Texniccenter, Notepad++/Atom editors (requires a little more effort to get it running but very useful for general writing needs for all languages Py, R, C as it can auto-detect language and syntax, making it a versatile solution). LyX is also an often-used latex editor which is more like a document (word) processor where you can write LaTeX documents assisted with a graphical interface. I gave it a try some time ago and it did not provide the writing flexibility I was looking for as was available with Texmaker.

## Speed-writing Tools to Save Time

Over the years, I have utilized available tools (thanks to peers who have saved and shared those over the internet), to make tables, convert powerpoints to Beamer (slide shows using LaTeX), MS-Excel to LaTeX, MS-Word to LaTeX,  and LaTeX to MS-Word. These tools saved me a lot of time and I hope it saves your precious time; allowing you to focus on writing than worrying about the writing method. I enlist some of these resources with a short review and more importantly there links.

### LaTeX Tables

1. Excel2LaTeX: Making tables in LaTeX can be tedious, especially if some columns are calculated. This converter allows you to write a table in Excel instead, and export the current selection as LaTeX markup which can be easily pasted into your existing LaTeX document.

2. Online Table Generator: I frequently use this when I need to create smaller tables with very few formatting needs. This is a quick method of creating Tables very easily. Note that you can even copy tabular data into online cells and format before you create the table. The only issue is you cannot do calculations like you would in Excel.

## LaTeX to Word (or back) or Powerpoint Conversion

1. GrindEq: Convert your MS-Word documents to LaTeX, it also allows you to convert your LaTeX documents to MS-Word (there is an easier/faster way for this).

2. Adobe Acrobat Pro: Allows you to convert PDF to Word. So, you can easily convert your final LaTeX document to MS-Word free, although it is not very good with preserving mathematical notations (as it converts them from image to text) and also for formatting.

3. Google Docs: Allows you to convert PDF to Word. So, you can easily convert your final LaTeX document to MS-Word or Google Docs for free. Again, since it is an OCR processor like Adobe, the final output will not be perfect. The best I have seen is GrindEq.

4. Writer2LaTeX: Works with OpenOffice (LibreOffice) and helps you to convert a word document to LaTeX for free. Does a decent job.

5. PanDoc: is a very versatile file converter allowing conversion between WORD(RTF)-LaTeX-PowerPoint-PDF using MikTeX. However, I found it not so easy to install and use. Although, the final output for converting files was the most superior (clean) among all the suggested methods here as it uses MikTeX. Goods news – it is FREE to install and you can try it here!

6. PowerPoint to Beamer:  I like to present using Beamer. Beamer can automatically put a little index at the top of my slides so people know where I am going, and the default fonts and colors work well. Most importantly, a lot of my research is mathematical in nature, and presenting mathematical equations with PowerPoint is tedious. There is MathType – paid, and a free TeX plugin: IguanaTeX, but Beamer is better as it also takes care of formatting and indexing. The tool I use is a VBA code (Macro) that needs to be run from within a PowerPoint document, saved as an RTF document. This converts all slide text to a beamer file as well as extracts all the images (indexed well) in a folder for use with your Beamer LaTeX presentation. I have used this often for preparing my own class presentations with publisher slides. You can find more details at https://jasonkerwin.com/nonparibus/2018/02/21/quickly-convert-powerpoint-slides-beamer-indent-code-nicely/

## License

Copyright 2016-present [Varun Gupta](https://personal.psu.edu/vxg15/).