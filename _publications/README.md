# Adding a publication

## Create the html file + assets folder

`<KEY>` of a submission should be `YYYY-MM-TITLE` where title is a short key for your paper. Year and month should be the **conference date**, not the upload date.

1. Create a new `<KEY>.html` file in the `_publications` directory. 
2. And create a folder named `<KEY>` in `/assets/publications/<KEY>` which will contain all files for this publication.
3. Add all files to this directory, this is where
4. Upload all videos to the **lab youtube account**

Complete the file with the following basic format.

```html
---
layout: article

date: YYYY-MM-DD
title: "..."
authors:
  - ...
  - ...
venue: ...
type:
  - Conference
  - Full Paper
  - Peer-reviewed
tags: 
  - ...
awards:
  - ...

video: "https://youtu.be/L6lUH0r-w-o"
video-preview: "https://youtu.be/8bmEJSOBm_U"
video-thumb: "https://youtu.be/8bmEJSOBm_U"

image: teaser.png
image-thumb: thumb.png

pdf: paper.pdf
doi: add full doi url

external-urls: 
  - ...
external-names:
  - 
external-types:
  - link
  - download
  - document
  - video
  - git-code
  - code
  - deploy

page-title: "..."
page-subtitle: "..."
---

Content of the project page in **HTML**. add all assets and files that are used in the folder `/assets/publications/KEY` and refer only to the filenames. 

```

## Mandatory fields
- `publication-date: YYYY-MM-DD` the date of the publication (e.g. of the conference), this value is used for sorting
- `title:` the paper title
- `authors`: all authors as a list
- `pdf:` the filename of the paper for download, which is located in "/assets/publications/KEY/"
- `image:` the filename of the banner-style teaser image that is shown on the project page, which is *min. 1200 px* wide, *max. 300 kB* and located in "/assets/publications/KEY/"
- `venue:` full publication venue, as it will be shown on the website (e.g. "In Proceedings of ACM CHI’19. Glasgow, UK, May 4 – 9, 2019.").
- `video-thumb` and/or `image-thumb`. this thumbnail will be shown in the publications list. use the video-thumb (typically the 30s preview) whenever possible. the image-thumb should be *16:9, min. 560 x 315 px* and *max. 60 kB*.  
- `type: ` the type of the publication. below are the available types. if new ones are necessary, please add them to this README so others can use them as well.
  - Conference
  - Journal
  - Full Paper
  - Short Paper
  - Workshop Paper
  - Demonstration


### If applicable
- `awards:` all awards as list

## Highly encouraged
- `doi:` add the full link, e.g., https://dl.acm.org/doi/10.1145/3290605.3300877
- `video:` the link to the submission video. upload to the lab YOUTUBE account, click share and paste that URL.  (example: "https://youtu.be/iy8CKbDlS5c")
- `video-preview:` the link to the ~30 sec preview video. upload to the lab YOUTUBE account, click share and paste that URL.  (example: "https://youtu.be/iy8CKbDlS5c")


### Optional
- `page-title:` if the paper title is too long, you can optionally use this tag to set a different page title. the paper title in `title` will still be used for the publications list
- `page-subtitle:` you can add the rest of the paper title as subtitle.


### External links (is applicable)
The external links can be anything that points to more resources. The 3 lists are combined index-based. These can be **slides, talk recording, source code, deployed application, etc.**
- `external-urls:` a list. e.g. URL_1, URL_2
- `external-names:` the display names of the urls, e.g., "try our editor", "slides" 
- `external-types:` the type of the link which defines the button icon, e.g. deploy, download. available link types are 
  - "link"
  - "download"
  - "document"
  - "video"
  - "git-code"
  - "code"
  - "deploy"

THe example links would be: (1) [try our editor](URL_1) of the type "deploy", (2) [slides](URL_2) of the type "download".


## Please keep the images small for fast loading
It's important that we keep all file sizes *small*. Please use https://tinypng.com/ to reduce the file sizes af all images.
