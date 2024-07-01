---
layout: post
title: Tips on open source scientific illustration
date: 2024-06-26
description: Some useful resources for making figures and cartoons
tags: illustration, figures
categories: resources
---

Clearly communicating our work via figures and cartoons is an essential part of any scientist's job. Clear, easy to read graphs, allow colleagues to clearly understand what we have discovered far more quickly than dense, poorly labelled ones. Explanatory cartoons - even if they are not works of art! - allow colleagues to understand the models we propose much more easily that text alone.

Pragmatically, clear visual communication also helps enormously when submitting manuscripts to selective journals or writing grant applications.

## Scientific graphic design books
- [The Visual Display of Quantitative Information](https://www.edwardtufte.com/tufte/books_vdqi) by Edward Tufte is the classic book on how to communicate scientific data visually. This book taught me most of what I know about figure design. At its core is an appeal for visual minimalism - use only as much explanatory info ("chart ink") as necessary - no more! The core maxim is "Maximise the data ink to chart ink ratio". 
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/tufte_vdqi_bookcover.gif" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- Reading any general graphic design textbook is also extremely helpful to cover basic principles like composition and colour. I like [Design Elements, A Graphic Style Manual](https://www.google.co.uk/books/edition/Design_Elements/zipdUxzimyoC?hl=en&gbpv=0) by Timothy Samara.

## Recommended software for scientific illustration
- [Inkscape](https://inkscape.org/) is a free and open source illustration software for vector graphics. Vector graphics means that the basic components of the image are lines and shapes, so when you zoom in, the image does not get blurry or pixelated, instead the computer draws it at higher resolution. This is ideal for arranging and editing data figures and making cartoons. It is not useful for editing photos. The functionality it offers is similar to Adobe Illustrator.
	- There is a very useful Inkscape extension called [Scientific Inkscape](https://github.com/burghoff/Scientific-Inkscape) which I recommend installing via *Extensions\>Manage Extensions* in Inkscape. It allows easy resizing, cleaning up and minor editing of graphs imported from Python, MATLAB and similar sources.
- [FIJI/ ImageJ](https://imagej.net/software/fiji/) is free and open source software for analysing and editing scientific images made up of pixels, ie photos and micrographs. Using FIJI is strongly recommended above photo editing software such as GIMP or Photoshop as it is designed with good digital image ethics in mind. You can use FIJI to do common tasks like adjusting image contrast (within appropriate limits!) and adding scale bars. I recommend exporting processed images in *PNG format* for subsequent use as figure panels in Inkscape.
- *Python, MATLAB or R to prepare graphs*. Python or R are preferred as they are open source, but if you are a dinosaur like me and still use MATLAB, it can also prepare excellent quality figures. The key requirements are that your graphing software must be able to export graphs in a *vector format* such as PDF or SVG and that they should be able to make the graphs as high quality as possible such that they require only minimal final editing (such as resizing/ reshaping) in Inkscape.


## Other scientific image/ data software
- [GIMP - GNU image manipulation program](https://www.gimp.org/) is a free and open source illustration software for raster graphics. Raster graphics means that the basic components of the image are pixels, like in a photo. When you zoom in the image becomes pixellated. The functionality it offers is similar to Adobe Photoshop. This software is principally for editing photos, which is actually not all that useful because most of the photos we use in science are *data* such as micrographs or western blot scans, and the allowable set of edits that can be made to scientific images is [very small](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4210356/). Usually, FIJI/ ImageJ (above) is a much better choice. I have used GIMP a few times to make artworks such as journal cover submissions.
- There are several good alternatives for graphing that are not free/ open source but which are nevertheless very useful. *Microsoft Excel* is fine for quick and dirty analyses, and can export vector format charts, but generally is not optimal for scientific analyses and the graphs need a lot of work to be made at all attractive. I have had very positive experiences with *GraphPad Prism* in particular for teaching undergraduates, as it avoids the need for any coding while performing high quality analyses and figures. If you are at Masters level or above though, I strongly recommend learning Python or R.
- *Biorender* can make excellent illustrations with little effort, mostly because it contains an extensive proprietary library of scientific clip art. I am not that big a fan of it though, partly because their licenses are quite restrictive - eg they require  exceptional permission to use their figures in open access manuscripts, see also [this tweet](https://x.com/baym/status/1779186456189124877) - but *mainly* because they do not offer any option for exporting their images in vector format. Only raster formats are offered, which makes it hard to then integrate good quality cartoons into larger figures prepared with Inkscape or other vector graphics software. Biorender Pro users have the option in Biorender to export to PDF, but this is not a vector PDF, it is just a PDF wrapper around the underlying bitmap. I suppose they are worried about losing control of their proprietary clipart library, which I understand, but it is quite annoying and limiting.

## Open clip art and image libraries useful for science
There are several really excellent sources of scientific images made freely available, which can be incorporated into your cartoons and diagrams. See note below about licenses and attribution.
- [BioIcons](https://bioicons.com/) - Lots of high quality biology focussed clip art cartoons or diagrams in vector format (SVG), eg cells, organs. Mostly released under CC-BY or CC0.
- [SciDraw](https://www.scidraw.io/) - Lots more excellent biology focussed vector format clip art (SVG), similar to BioIcons. CC-BY license.
- [Smart Servier Medial Art](https://smart.servier.com/) is a library of 3000 free medical images - very high quality and very detailed - released by the [Servier Laboratories](https://servier.com/). The illustrations are mostly cartoons (vector format) but the default download format is either PNG (raster) or PowerPoint. Happily, the PowerPoint files contain the vector format images. To export these in vector format, download the PowerPoint and export the page containing the relevant illustration as a PDF. This PDF can then be opened and edited in Inkscape or other Vector editor. Also note after import in Inkscape you may need to remove an additional imported page behind the image using the *Pages Tool*. CC-BY license.
- University of Maryland [Center for Environmental Science Media Library](https://ian.umces.edu/media-library/). A collection of vector cartoons and raster photos, focussed on environment and ecology. CC-BY-SA license.
- [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page). A huge collection of  vector cartoons and raster photos on broad topics. Licenses depend on the image and should be checked, but are usually CC-BY, CC-BY-SA, CC-0 or public domain.

Note that Inkscape has a tool to directly import clipart from several of above websites, but browsing using it is a little bit slow, so I would recommend directly searching the above sites, downloading the SVGs of interest and importing them manually.

## Licenses and attribution
It is essential that you properly attribute and acknowledge the use of any third-party content in your figures and artwork. Usually, this can be done in the acknowledgements section of a paper, or eg at the bottom of a PowerPoint slide. Some licenses (see below) do not legally require such attribution, but good academic practice requires that any content not created by the author *must* be clearly acknowledged.

Typically an appropriate acknowledgement could look something like "Third party graphical elements were incorporated into the indicated figures, from the cited sources under the indicated license: Figure 2A, Refs \[3,6\], CC-BY and public domain, Figure 3D, Ref \[7\] CC-0, Figure 5C, Ref \[8\], CC-BY-SA. Per the requirements of the CC-BY-SA license, Figure 5C is made available under a CC-BY-SA licenses." Hopefully the above should make more sense in a minute. 

There are a few common licenses under which artwork is typically made available online.
- *Full copyright retention/ commercial license*: The default is standard author copyright, often used by professional photographers and illustrators - if you want to use their work, you must pay them. If you do engage a professional, you should still acknowledge their work. Example acknowledgment: "Third party graphical elements created by *ExampleIllustrator* were incorporated into Figure 6". If you are publishing in an open access journal, the illustrator would still need to give their permission for the art to be released under a CC-BY license.
- *Public domain*: At the other extreme, public domain works are those where the author has explicitly renounced all rights to the image, and there are no restrictions on its use. However you should still acknowledge the source. Example acknowledgment: "Third party graphical elements were incorporated into Figure 6 from Ref \[9\] under public domain license".
- [Creative Commons](https://creativecommons.org/share-your-work/cclicenses/) open licenses. These licenses allow free reproduction and usually allow further editing but with certain constraints. Ones that you will commonly encounter are:
	- *CC-0*: This license does not require attribution, however as an academic you should still acknowledge the work. Example acknowledgement: "Third party graphical elements were incorporated into Figure 6 from Ref \[9\] under CC-0 license".
	- *CC-BY*: This license requires attribution. Example acknowledgement: "Third party graphical elements were incorporated into Figure 6 from Ref \[9\] under CC-0 license".
	- *CC-BY-SA*: This license requires attribution *and artwork incorporating these graphics must be released under the same license* or another compliant open source license. Example acknowledgement: "Third party graphical elements were incorporated into Figure 6 from Ref \[9\] under CC-BY-SA license. Figure 6 is released under a CC-BY-SA license".

It can be helpful to keep track of the sources of any clipart that you use by adding that information to the metadata of your image. Eg in Inkscape, you can manually add the source information as text in *File\>Document Properties\>Metadata\>Description*.

## Some brief tips
- I always start cartoons by making a hand drawn sketch in pencil, biro and/ or marker. This enables me to quickly iterate how the cartoon should look and if it makes sense. Also, as a fallback if I am very pressured for time, eg. for a talk, there is always the option of using good hand drawn illustrations as a pretty OK cartoon until I get the chance to make a publication quality figure on the computer.
- Be mindful of the final dimensions of your image. If it is a journal figure, will it be one or two columns, and how much of the page will it take up? If it is going in a PowerPoint slide, how much of the slide will it take up. If you can set the dimensions of the page appropriately in Inkscape, eg to A4, and then ensure that the Figure matches the expected final dimensions reasonably well, you should not need to resize the final figure - in particular this  will mean that the font sizes remain reasonable.
- Good figure font sizes to aim for are 8-pt for panel labels, and 5-7-pt for all other figure elements.
- Nature Publishing Group have some good [guidelines](https://www.nature.com/documents/Final_guide_to_authors.pdf) on how to format high quality figures which apply equally well to almost any journal.
- All your micrographs should contain scale bars. Here's a good tip adapted from advice  from Christophe Leterrier: when exporting from FIJI, make two copies of the image, one with hardcoded scale bar, one without. Then import both to Inkscape (or Illustrator per Christophe's workflow), draw a rectangle over the hardcoded scalebar, move it onto the image without the hardcoded scalebar, and group the image + scalebar so that any resize affects both the same. Voila - now you can reposition the scalebar or change its thickness instead of having to go back to FIJI to update it.
- Important Inkscape defaults for figure import/ export: Microscopy images should be imported using the *ImageScale\>Blocky* option - this means that when you resize an image, it does not blur it, it just makes the original pixels bigger. Default export resolution should be at least 300dpi. Change these settings in *Edit\>Preferences\>Input/Output\>Imported Images*, or in the import or export dialogues.
- Learn the basic Inkscape shortcuts! Here's a basic [cheat sheet](https://logosbynick.com/inkscape-keyboard-shortcuts-2/).
- On the subject of Inkscape shortcuts, if you are already experienced with another illustration software and want to move over, you can keep the shortcuts you are used to, eg. Illustrator or CorelDRAW. See *Edit\>Preferences\>Interface\>Keyboard*.
- A really good tip that I use often is - if you like the visual style of a cartoon or even the layouts of figures in a paper, do not be afraid to imitate them! 
- Some of my favourite figures use little cartoons throughout to explain or interpret the data in situ, eg with little cartoons of phenotypes inline with images. The easier you can make your figure to interpret the better.

## Helpful Inkscape resources
- [https://inkscape.org/learn/](https://inkscape.org/learn/)
- [https://inkscape-manuals.readthedocs.io/en/latest/#](https://inkscape-manuals.readthedocs.io/en/latest/#)
- [Inkscape for scientists](https://www.youtube.com/playlist?list=PLxtauMB7RON_2tg-mRQTuieFUr29IOKzW) - A very good playlist of Youtube videos that takes you through Inkscape basics for making figures and cartoons.
- [Decent tutorial on the toolbars in Inkscape v1.3 (latest version)](https://www.youtube.com/watch?v=jlhFFsV7JLk)
- [Draw a coffee cup in Inkscape](https://www.youtube.com/watch?v=geo4UnxFAmw) - good practical Inkscape tutorial, it uses a little bit of an old Inkscape version but hits the core techniques

Author: Séamus Holden
