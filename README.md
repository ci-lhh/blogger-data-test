# blogger-data-test
Provide easily-importable, sufficiently-diverse sample data for exploring and testing Google Blogger blogs, themes, layouts and widgets across the 4 types of views generated: index (items, tags, search results), static page, item (post), and archive. A 404 error page is unaffected by blog data.

[ See https://github.com/ci-lhh/blogger-data-test ]

[See https://github.com/matiassingers/awesome-readme ]

.

## Features
 - XHTML file containing importable blogger data set with pages, posts, and comments
   - random [lorem ipsum text](https://www.lipsum.com/) content
   - variety of [random images](https://randomwordgenerator.com/picture.php) for page and post headers, occasional images embedded in content paragraphs, plus a few images following content
    - 8 pages
        - comments
            - allows testing of comments allowed, no new comments, and comments hidden settings
            - comments and replies to comments (nested comments)
    - 12 labels (category tags) helps testing of displays of individual posts and posts by label
    - 33 posts
        - many recent posts with fewer during the preceding 4 years (i.e. randomized front-loaded timestamps between 2019-04-22 and 2022-09-22) allowing testing of various archive settings
        - variety of label assignments (none, up to 5)
        - variety of descriptions (for meta tag generation and associated search results)
        - most posts contain [randomized locations in the United States](https://hiveword.com/location-name-generator)
        - all posts (except one) have a header image, with posts containing a variety of random images; some embedded in paragraphs, some following paragraph content. All images have alternate descriptions.
        - 2 paragraphs per post
        - single stylesheet post used to view a [variety of HTML elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#inline_text_semantics) (e.g. text that is bold, italicized, underlined, emphasized, highlighted, struck, subscript, or superscript; anchors; links; lists that are ordered, unordered or definitions; subscript or superscript; inline or block quotes; citations; abbreviations; horizontal rules; figures; preformatted text; code; keyboard input; mathematical formulas; etc.)
        - 148 comments
            - allows testing of comments allowed, no new comments, and comments hidden settings
            - comments and replies to comments (nested comments)

 - [Google sheet with raw data](https://docs.google.com/spreadsheets/d/1xrcaOy78e8cxkBVDXFVFinEe_0Yiyr62U65jl9zF4R0/edit?usp=sharing) can be copied (or included Microsoft Excel spreadsheet can be used) to access raw data and build additional data for test pages, posts, and labels.

## Background
While exploring the creation of themes for [Google Blogger](https://www.blogger.com/) using various sections, layouts, and widgets, discovered there was not enough data (e.g. pages, posts, or labels) with enough diversity to clearly understand how information would be displayed to visitors. Wanted to focus on Google products to explore integration of various [Google Cloud](https://cloud.google.com/) modules as tools for community members.

## Requirements
 - Existing Google Account (e.g. GMail)
 - Ability to comfortably navigate GitHub website
 - Ability to comfortably navigate Google Blogger website

## Installation
1. [Sign-in to Google account](https://accounts.google.com/)
1. Go to [Google Blogger](https://www.blogger.com/)
1. Click drop-down box at top of left-hand sidebar
1. Select `New Blog…`
1. Enter title for test blog (e.g. My Blog Template Testing)
1. Enter subdomain address for test blog (e.g. mytest2058)
1. Click `Settings` near bottom of left-hand toolbar
1. Scroll down to `Manage Blog` section
1. Select `Import content`
1. On pop-up window, click `IMPORT` button
1. Select downloaded `blogger-data-test.xml` file

## Configuration
--TODO--

## Usage
--TODO--


## Test Case Highlights
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


## Support
--TODO--

## Authors and Acknowledgment
--TODO--

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Roadmap
--TODO--

## License
[MIT](https://choosealicense.com/licenses/mit/)
