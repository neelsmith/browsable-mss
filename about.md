---
layout: page
title: About this site
---

## The goals of this site

Literally thousands of Greek and Latin manuscripts are now documented in high-quality, openly licensed digital images that are readily accessible over the internet.

The primary goals of this site are:

1. to offer simple browsable facsimiles of a selection of manuscripts and papyri that let you cite surfaces and documentary images using technology-independent, immutable URNs
2. to provide a simple, documented method for creating citable facsimile editions that can be added to this site or easily used in a docker container


## 1. Citable facsimiles

Browsable facsimile views let you navigate forward and backward through a codex either page by page, or by bifolio spread (depending on the layout of the manuscript).  You can directly open a page from a visual table of contents with thumbnail images of each manuscript, from a pop-up menu listing each page, or even by manipulating the URL in your browser. By appending subdirectories to the base URL <https://browsable-mss.netlify.app/mss/> corresponding to the namespace, group, version, and object identifier of a URN, you can directly map the URN to its address here. For example, *Iliad* 24 begins on folio 250 recto of the "Townley Homer."  The URN for this page is `urn:cite2:citebl:burney86pages.v1:250r` so on this site you will find it at <https://browsable-mss.netlify.app/mss/citebl/burney86imgs/v1/250r/>.

The facsimile files are simple static markdown files that include a URN identifying the page or bifolio spread, and an image linked to the Homer Multitext project's Image Citation Tool so that you can also easily cite regions of the documentary image.  Combining citation of a surface and an image lets you model a codex or papyrus roll; add your own canonically citable diplomatic text and you can model a full diplomatic edition with visual evidence for its supporting artifact.


## 2. Building citable facsimiles

With removable storage in the terabyte range affordable many individual users,  convenient tools like Ryan Baumann's downloading utilities [iiif-dl](https://github.com/ryanfb/iiif-dl) and [dzi-dl](https://github.com/ryanfb/dzi-dl), and a solid infrastructure for packaging specialized packages in Docker images, it's straightforward to create a citable facsimile edition.

In the [data section](./data/) of this web site, I document the steps taken to create citable facsimile editions from different freely available sources of images, and link to accompanying catalogs of images and codex pages in simple delimited-text files.

Like the facsimiles, the documentation of data sources is organized in subdirectories corresponding to URN components.  For information on how to download images from the British Museum, the URL is therefore <https://browsable-mss.netlify.app/data/citebl>, and for the Homer Multitext project it is <https://browsable-mss.netlify.app/data/hmt>.
