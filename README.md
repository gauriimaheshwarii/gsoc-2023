<div align="center">

<img src="assets/gsoc.png" height="auto" width="600" />
<br />

<img src="assets/freeCAD.png" height= "auto" width="400" />
<br />

<h1> Google Summer of Code 2023 </h1>
<h2> FreeCAD </h2>

</div>

## Table of Contents

- [About FreeCAD](#about-freecad)
- [Introduction](#introduction)
- [Project Team](#project-team)
- [Work Summary](#work-summary)
- [Future Work](#future-work)
- [Challenges](#challenges)
- [Acknowledgments](#acknowledgments)
- [References](#references)
- [Help, Feedback, and Contribute](#help-feedback-and-contribute)

## About FreeCAD

- FreeCAD is a general-purpose parametric **3D computer-aided design (CAD) modeler** and a Building Information Modeling (BIM) software application with Finite-Element Method (FEM) support.  
- It is intended for mechanical engineering product design but also expands to a broader range of uses around engineering, such as architecture or electrical engineering.  
- FreeCAD is free and open-source, under the **LGPL-2.0-or-later** license, and available for Linux, macOS, and Windows operating systems.  

## Introduction

FreeCAD possesses a vast amount of documentation that is written by its users and hosted on the [FreeCAD Wiki](https://wiki.freecad.org/). The entire documentation is currently managed by MediaWiki software, which faces several problems and poses a potential threat.  

1. The MediaWiki software is massive and therefore, it becomes difficult and complicated to maintainup-to-date.
2. The data published on MediaWiki is hard to backup, so there is a constant risk of losing data.
3. The search feature supported by MediaWiki is extremely weak.

The FreeCAD documentation is as important as the software, and it  would benefit from the same level of decentralization.  

The **aim** is to rework the documentation system to a simple, file-based,versioned system that supports Git and Markdown for easy editing and version control, and to offer the FreeCAD users a good web-based experience with a robust search system.

## Project Team

- Contributor: Gauri Maheshwari - [GitHub](https://github.com/gauriimaheshwarii) | [LinkedIn](https://www.linkedin.com/in/gaurimaheshwari/) | [X](https://twitter.com/gaurii09)
- Mentors:
  - Kurt Kremitzki - [GitHub](https://github.com/kkremitzki) | [LinkedIn](https://www.linkedin.com/in/kurt-kremitzki-12524919/) | [X](https://twitter.com/thekurtwk)
  - Chris Hennes - [GitHub](https://github.com/chennes) | [LinkedIn](https://www.linkedin.com/in/chrishennes/) | [X](https://twitter.com/chrishennes)
- Organization Admin: Yorik van Havre - [GitHub](https://github.com/yorikvanhavre) | [LinkedIn](https://www.linkedin.com/in/yorik/) | [X](https://twitter.com/yorikvanhavre)

## Work Summary

### Offline documentation support

- Users can also make a PDF copy of the documentation by running the command:

```
npx docs-to-pdf --initialDocURLs="https://freecad-documentation.netlify.app/docs/intro" --contentSelector="article" --paginationSelector="a.pagination-nav__link.pagination-nav__link--next" --excludeSelectors=".margin-vert--xl a,[class^='tocCollapsible'],.breadcrumbs,.theme-edit-this-page" --coverImage="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/FreeCAD-logo.svg/96px-FreeCAD-logo.svg.png?20230430105342" --coverTitle="FreeCAD Documentation" --outputPDFFilename="freeCAD-documentation.pdf"
```

### CLI options for PDF generation

| Option | Required | Description |
| - | - | - |
| --initialDocURLs | Yes | Set URL to start generating PDF from |
| --contentSelector | Yes | Used to find the part of main content |
| --paginationSelector | Yes | CSS Selector used to find next page to be printed for looping |
| --excludeURLs | No | URLs to be excluded in PDF |
| --excludeSelectors | No | Exclude selectors from PDF. Separate each selector **with comma and no space**. But you can use space in each selector. <br> **ex**: `--excludeSelectors=".nav,.next > a"` |
| --cssStyle | No | CSS style to adjust PDF output <br> **ex**: `--cssStyle="body{padding-top: 0;}"` |
| --outputPDFFilename | No | Name of the output PDF file <br> default is `freeCAD-documentation.pdf` |
| --pdfMargin | No | Set margin around PDF file. <br> separate each margin **with comma and no space**. <br> **ex**: `--pdfMargin="10,20,30,40"`. <br> This sets margin top: 10px, right: 20px, bottom: 30px, left: 40px |
| --coverTitle | No | Title for the PDF cover |
| --coverSub | No | Subtitle the for PDF cover. <br> Add `<br/>` tags for multiple lines. |
| --filterKeyword | No | Only adds pages to the PDF containing a given meta keywords. <br> Makes it possible to generate PDFs of selected pages. |

> For more information on CLI options, refer [here](https://www.npmjs.com/package/docs-to-pdf).

## Future Work

## Challenges

## Acknowledgments

## References

- [New documentation](https://freecad-documentation.netlify.app/)
- [Project page](https://summerofcode.withgoogle.com/programs/2023/projects/iPaw5Jd9)
- [Issue link](https://github.com/FreeCAD/FreeCAD/issues/8558)
- [Project repository](https://github.com/FreeCAD/FreeCAD-documentation-docusaurus)
- [Forked repository](https://github.com/gauriimaheshwarii/FreeCAD-documentation-docusaurus)

## Help, Feedback, and Contribute

- [FreeCAD Forum](https://forum.freecad.org/)
- [GitHub](https://github.com/FreeCAD/FreeCAD)
- [X](https://twitter.com/FreeCADNews)
- [LinkedIn](https://www.linkedin.com/groups/4295230)
- [IRC Channel](irc://chat.freenode.net/freecad)
- [Discord](https://discord.com/invite/w2cTKGzccC)
- [Facebook](http://www.facebook.com/FreeCAD)
- [Mastodon](https://fosstodon.org/@FreeCAD)
- [Gitter](https://gitter.im/FreeCAD/FreeCAD)
- [Reddit](https://www.reddit.com/r/freecad)
- [Bugs Tracker](https://github.com/FreeCAD/FreeCAD/issues)
