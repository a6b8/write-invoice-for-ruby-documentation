---
sort: 1
title: A. Header
---

# Section: Header

The origin position of this section is on top of the page and can include a logo and other company defaults.


## Preview

<div >
    <canvas id='canvas' search='header' palette='section_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  
 

## Options

| **Nr** | **Name** | **Key** | **Default** | **Description** |
| :--- | :--- | :--- | :--- | :--- |
| [A.7](/options/#show) | [Show Logo](/options/show__logo) | :show__logo | `false` | Show or Hide Logo. To set your Image path or base64 string visit [headline__image__src](../options/headline__image__src.html) |
| [A.9](/options/#show) | [Show Unencrypted](/options/show__unencrypted) | :show__unencrypted | `true` | Encrypt or unencrypt .pdf document. To set a password visit [Payload](../payload/#example) #example > document > encrypted |
| [C.7](/options/#text) | [Text Page Count](/options/text__page_count) | :text__page_count | `<page> / <total>` | Set Page count output here. Use `<page>` to show current page number and `<total>` to show sum of all pages. |
| [D.2](/options/#style) | [Style Page Count Align](/options/style__page_count__align) | :style__page_count__align | `right` | Set Page Count alignment |
| [D.3](/options/#style) | [Style Page Count Start Count At](/options/style__page_count__start_count_at) | :style__page_count__start_count_at | `1` | Start to count from. |
| [D.4](/options/#style) | [Style Page Count Offset Y](/options/style__page_count__offset_y) | :style__page_count__offset_y | `0` | Set an `y offset` for page count string. |
| [D.10](/options/#style) | [Style Colors Header Default](/options/style__colors__header__default) | :style__colors__header__default | `000000` | Set background color for header section |
| [D.13](/options/#style) | [Style Header Height](/options/style__header__height) | :style__header__height | `90` | Set total height of header section. |
| [F.29](/options/#sections) | [Sections One Name](/options/sections__one__name) | :sections__one__name | `{:content=>nil, :struct=>"<b><<--a-->></b>\n<<--b-->>\n<<--c-->>\n<<--d-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__from__address__phrase, :format=>nil}, {:value=>:payload__from__address__city, :format=>nil}, {:value=>:payload__from__address__country, :format=>nil}]}` | Define text in section "one" (header) |
| [G.1](/options/#headline) | [Headline Grid X](/options/headline__grid__x) | :headline__grid__x | `3` | Set grid size on the `x axis`. |
| [G.2](/options/#headline) | [Headline Grid Y](/options/headline__grid__y) | :headline__grid__y | `1` | Set grid size on the `y axis`. |
| [G.3](/options/#headline) | [Headline Default Content](/options/headline__default__content) | :headline__default__content | `` | `Autofill` every cell with content if you wish. |
| [G.4](/options/#headline) | [Headline Default Style](/options/headline__default__style) | :headline__default__style | `style__document__font_size__small` | Set `font style` as a reference. |
| [G.5](/options/#headline) | [Headline Default Align](/options/headline__default__align) | :headline__default__align | `right` | Set default aligment behaviour of text. |
| [G.6](/options/#headline) | [Headline Default Text Color](/options/headline__default__text_color) | :headline__default__text_color | `style__colors__header__default` | Set `default text` color in section "one" (headline). |
| [G.7](/options/#headline) | [Headline Default Borders](/options/headline__default__borders) | :headline__default__borders | `[:left]` | Set `border type` in section "one" (headline). |
| [G.8](/options/#headline) | [Headline Default Border Width](/options/headline__default__border_width) | :headline__default__border_width | `2` | Set `border width` in section "one" (headline). |
| [G.9](/options/#headline) | [Headline Image Src](/options/headline__image__src) | :headline__image__src | `` | Set local `image path` for company logo, use .png or .jpg |
| [G.10](/options/#headline) | [Headline Image Colspan](/options/headline__image__colspan) | :headline__image__colspan | `2` | Set how many cells in the `columns (x)` direction should be merge to show the image. |
| [G.11](/options/#headline) | [Headline Image Rowspan](/options/headline__image__rowspan) | :headline__image__rowspan | `2` | Set how many cells in the `rows (y)` direction should be merge to show the image. |
| [G.12](/options/#headline) | [Headline Image Grid](/options/headline__image__grid) | :headline__image__grid | `[0, 0]` | Set start position `[ columns x, rows y ]` of image. |
| [G.13](/options/#headline) | [Headline Image Borders](/options/headline__image__borders) | :headline__image__borders | `[]` | Set `border type` of image cell. |
| [G.14](/options/#headline) | [Headline Image Fit](/options/headline__image__fit) | :headline__image__fit | `[160, 100]` | Use `fit size` to adjust the image. |
| [G.15](/options/#headline) | [Headline Image Border Width](/options/headline__image__border_width) | :headline__image__border_width | `0` | Set `border width` of image cell. |
| [G.16](/options/#headline) | [Headline Texts](/options/headline__texts) | :headline__texts | `[{:content=>:sections__one__name__content, :grid=>[2, 0], :style=>:style__document__font_size__h1, :align=>:right, :text_color=>:style__colors__header__default, :borders=>[], :border_width=>0}]` | Set a reference to `string data`. |


