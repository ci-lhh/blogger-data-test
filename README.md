# blogger-data-test

Provide easily-importable, sufficiently-diverse sample data for exploring and testing Google Blogger blogs, themes, layouts and widgets across the 4 types of views generated: index (items, tags, search results), static page, item (post), and archive. A 404 error page is unaffected by blog data.

[ See https://github.com/ci-lhh/blogger-data-test ]

[See https://github.com/matiassingers/awesome-readme ]

.

## Features

### Key Features

 - XHTML file containing importable Google Blogger data set with theme plus 9 pages (static pages), 12 category tags (labels), 34 posts (items), and 193 comments.
   - 9 pages with a variety of [titles](#titles), [descriptions](#search-descriptions), [body content](#bodies), and [comments](#comments);
   - 12 labels with a variety of [titles](#titles).
   - 34 posts with a variety of [timestamps](#post-timestamps), [titles](#titles), [descriptions](#search-descriptions), [labels (category tags)](#post-labels), [locations](#post-locations), [body content](#bodies), and [comments](#comments).
   - 193 [comments](#comments) (i.e. 53 for pages, 140 for posts).
 - Stylesheet page displays most common and most basic types of formatting using hypertext markup language (HTML) tagged content contained in bodies of blog pages and posts, including [headings](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), [addresses](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address), [text formatting](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#text_content), [inline semantics](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#inline_text_semantics), [demarcating edits](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#demarcating_edits), [tables](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#table_content), [multimedia](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#image_and_multimedia), [embedded content](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#embedded_content), and [forms](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#forms).
 - [Google sheet with raw data](https://docs.google.com/spreadsheets/d/1xrcaOy78e8cxkBVDXFVFinEe_0Yiyr62U65jl9zF4R0/edit?usp=sharing) can be copied (or included Microsoft Excel spreadsheet can be used) to access raw data and build additional data for test pages, labels, and posts.


### Content Features

#### Text

Random [lorem ipsum text](https://www.lipsum.com/).

#### Images

Variety of [random images](https://randomwordgenerator.com/picture.php) for:
 - page and post headers;
 - occasional embedding in [body paragraphs](#bodies); plus,
 - occasional inclusion after [body content](#bodies).

#### Titles

Single sentence of varying lengths containing random [lorem ipsum text](https://www.lipsum.com/).

#### Search Descriptions

Single sentence of varying lengths containing random [lorem ipsum text](https://www.lipsum.com/).

#### Bodies

[Random header image](https://randomwordgenerator.com/picture.php), followed by up to two paragraphs of varying lengths containing random [lorem ipsum text](https://www.lipsum.com/), followed by possibly up to two [random gallery images](https://randomwordgenerator.com/picture.php). Each image has alternate text with a single sentence of varying lengths containing random [lorem ipsum text](https://www.lipsum.com/). Each paragraph may or may not contain an embedded [random image](https://randomwordgenerator.com/picture.php). One or two posts do not have any images (i.e. no header image, no embedded paragraph images, and no post-content gallery images).

#### Comments

Variety of comments and replies (i.e. nested comments) on pages and posts to allow testing of comment permissions: allow; do not allow, show existing; plus, do not allow, hide existing. Each comment is a single sentence of varying lengths containing random [lorem ipsum text](https://www.lipsum.com/).

#### Post Timestamps

Many recent timestamps with fewer during the preceding 4 years (i.e. randomized front-loaded timestamps between 2019-04-22 and 2022-09-22) allowing testing of various archive settings.

#### Post Labels

Random selection of up to 5 labels from collection of 12 labels, whose titles contain up to 3 words of random [lorem ipsum text](https://www.lipsum.com/). One or two posts do not contain any label information.

#### Post Locations

Some posts contain a randomly chosen landmark in [a random city in the United States](https://hiveword.com/location-name-generator). Many posts contain only [a random city in the United States](https://hiveword.com/location-name-generator). A few posts only contain [a random state in the United States](https://hiveword.com/location-name-generator). One or two posts contain only the United States of America. One or two posts do not contain any location information. This variety helps test specificity of displayed locations.

.

## Background

While exploring the creation of themes for [Google Blogger](https://www.blogger.com/) using various sections, layouts, and widgets, discovered there was not enough data (e.g. pages, posts, or labels) with enough diversity to clearly understand how information would be displayed to visitors. Wanted to focus on Google products to explore integration of various [Google Cloud](https://cloud.google.com/) modules as tools for community members.

.

## Known Issues

### Google Blogger Backup (Export) / Restore (Import) Post and Page Entries Missing Search Description and Comment Permission Setting

When backing-up (exporting) the data from Google Blogger to create the XML file, the resulting XML file does not contain data for search description and comment permission settings in the post and page entries. Therefore, these missing data cannot be imported. See [related Blogger Help Community post](https://support.google.com/blogger/thread/182076325) for more information. See [Installation of Manual Workaround for Known Issues](#manual-workaround-for-known-issues).

.

## Requirements

 - existing Google Account (e.g. GMail)
 - ability to comfortably navigate GitHub website
 - ability to comfortably navigate Google Blogger website
 - ability to comfortably use basic hypertext markup language (HTML) to organize and format both text and images

.

## Installation

1. Clone repository to local workspace or download following files:
    - [blogger-data-test.xml](https://github.com/ci-lhh/blogger-data-test/blob/main/blogger-data-test.xml)
   - --TODO: blog logo --
   - --TODO: favicon --
1. [Sign-in to Google account](https://accounts.google.com/)
1. Go to [Google Blogger](https://www.blogger.com/)
1. Click drop-down box at top of left-hand menu sidebar
1. Select `New Blog…`
1. Enter title for test blog (e.g. My Blog Template Testing)
1. Enter subdomain address for test blog (e.g. mytest2058)
1. Click `Settings` near bottom of left-hand menu sidebar
1. Scroll down to `Manage Blog` section
1. Select `Import content`
1. On pop-up window, click `IMPORT` button
1. Select downloaded `blogger-data-test.xml` file

### Manual Workaround for Known 

1. If continuing directly from [Installation](#installation), skip to step #2, otherwise do following:
   1. [Sign-in to Google account](https://accounts.google.com/)
   1. Go to [Google Blogger](https://www.blogger.com/)
   1. Click drop-down box at top of left-hand menu sidebar
   1. Select title for test blog (e.g. My Blog Template Testing)

#### Post and Page Entries Missing Search Description and Comment Permission Setting

1. Click `Pages` near middle of left-hand menu sidebar
1. For each page in table below, do following:
   1. Select page title to load page for editing
   1. In right-hand menu sidebar, select `Search Description`
   1. Enter page search description from table below
   1. In upper-right-hand screen corner, click `Update` button
   1. In upper-left-hand screen corner, click `←` (back) button

   | Title | Search Description |
   | :---- | :----------------- |
   | Cras Quis Mauris Nibh. | Proin suscipit mi nibh, maximus aliquet lectus rutrum et. |
   | Duis Aliquet Ante Urna, Quis Vehicula Mauris Mollis Eu. | Aliquam efficitur laoreet nisl, et hendrerit dolor elementum quis. |
   | Maecenas Vestibulum Rutrum Mi At Molestie. | Etiam pretium luctus dolor, et lacinia risus molestie non. |
   | Sed Dignissim Eu Felis Ac Fringilla. | Etiam ut maximus massa. |

1. For each page in table below, do following:
   1. Select page title to load page for editing
   1. In right-hand menu sidebar, select `Search Description`
   1. Enter page search description from table below
   1. In right-hand menu sidebar, select `Options`
   1. Select page reader comments permission from table belowv
   1. In upper-right-hand screen corner, click `Update` button
   1. In upper-left-hand screen corner, click `←` (back) button
   
   | Title | Search Description | Comments Permission |
   | :---- | :----------------- | :------------------ |
   | Curabitur Imperdiet Dictum Sapien Non Commodo. | Ut eget mi ac eros congue fermentum. | Do not allow, show existing |
   | Nulla Blandit Non Ante In Mollis. | Lorem ipsum dolor sit amet, consectetur adipiscing elit. | Do not allow, show existing |
   | Aliquam Suscipit Sapien Vitae Tincidunt Mollis. | Morbi id ornare erat. | Do not allow, hide existing |
   | Morbi Bibendum Nisi Sed Tempor Ultrices. | Phasellus tincidunt erat quis lacus ultricies, vitae aliquam arcu elementum. | Do not allow, hide existing |

.

## Configuration

1. If continuing directly from [Installation](#installation), skip to step #2, otherwise do following:
   1. [Sign-in to Google account](https://accounts.google.com/)
   1. Go to [Google Blogger](https://www.blogger.com/)
   1. Click drop-down box at top of left-hand menu sidebar
   1. Select title for test blog (e.g. My Blog Template Testing)

1. Click `Settings` near bottom of left-hand menu sidebar
1. In `Basic` section, click `Description` item
1. On pop-up window, enter description (e.g. Sample blog for exploring and testing Google Blogger themes, layouts, and widgets.), then click `SAVE` button
1. --TODO: favicon --
1. Scroll down to `Comments` section, click on `Comment form message` item
1. On pop-up window, enter comment form message (e.g. Please share your reactions and thoughts with us! What did you like most? What could we improve?), then click `SAVE` button
1. Scroll down to `Formatting` section, click on `Time zone` item
1. On pop-up window, select your time (e.g. (GMT-05:00) Central Time – Chicago for CDT or (GMT-06:00) Central Time – Chicago CST), then click `SAVE` button
1. Scroll down to `Meta tags` section, click on slider to `Enable search description`
1. Click on `Search description`, then on pop-up window, enter website description to be used in search engine results (e.g. Sample blog for exploring and testing Google Blogger themes, layouts, and widgets.), then click `SAVE` button
1. Click `Layout` near middle of left-hand menu sidebar
1. Go through each of the sections (e.g. headers, sidebars, main, footers) and each of the included widgets to review all settings. Make sure all settings are enabled and have desired content (e.g. text or images) to help understand data that is available for visitors. For each widget, simply click pencil (edit) icon to view settings for widget.
   - If desired, get a random image for header widget at [Random Pictures](https://randomwordgenerator.com/picture.php)


--TODO--

.

## Usage

--TODO--

.

# Test Case Highlights

-- TODO: identify test case post dates --

✅❌
 - [Date] -- [Title]
   - info
 - 33 = latest post; multiple labels (5); long labels tag; full location (street, city, state, ZIP Code); long description tag; header image, image embedded in each paragraph, +2 additional post-content images; comments allowed (5 comments each with 5 replies (30 comments total))
 - 6 = earliest post; single label; header image plus each paragraph has images; multiple comments (4)
 - 21 = long post title
 - 25 = short post title; single label; short labels tag
 - 11 = no label; long location tag; no images; no new comments allowed, existing comments shown
 - 9 = no street, city, or state, only country location
 - 23 = no street, only city and state location; no new comments allowed, existing comments hidden (2)
 - 20 = single label; short description tag; header image only
 - 31 = very little paragraph content; header image, image for each paragraph, plus 1 post-content image; comments allowed, no comments posted
 - 3 = header image + 1st paragraph image; a lot of paragraph content; no new comments allowed, existing comments displayed (4)

.

## Support

--TODO--

.

# Authors and Acknowledgment

--TODO--

.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

.

## Roadmap

--TODO--

.

## License

[MIT](https://choosealicense.com/licenses/mit/)
