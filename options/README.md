---
sort: 4
title: Options
---

# Options
        

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
WriteInvoice::Document.generate( output: 'test.pdf', payload: pyld, options: {}, debug: true)
```

| Name | Type| Default | Required |
| :-- | :-- | :-- | :-- |
| `output:` | String | `nil` | no | 
| `payload:` | Hash | `{}` | yes |
| `options:` | Hash | `{}` | no |
| `debug:` | Boolean | `true` | yes | 

## Preview

<div >
    <canvas id="canvas" search="" palette="option_overview"></canvas>
</div>
<script src="../assets/js/marker.js"></script>

## Categories
### Show

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [A.1.](./show__qr_code) | [Qr Code](./show__qr_code) | :show__qr_code | `true` | [A](show__qr_code#example-a), [B](show__qr_code#example-b) | Show or Hide `QR Code` Image |
| [A.2.](./show__sub_total) | [Sub Total](./show__sub_total) | :show__sub_total | `true` | [A](show__sub_total#example-a), [B](show__sub_total#example-b) | Show or Hide `Sub Total` |
| [A.3.](./show__shipping) | [Shipping](./show__shipping) | :show__shipping | `true` | [A](show__shipping#example-a), [B](show__shipping#example-b) | Show or Hide `Shipping Row` |
| [A.4.](./show__total_net) | [Total Net](./show__total_net) | :show__total_net | `true` | [A](show__total_net#example-a), [B](show__total_net#example-b) | Show or Hide `Total Net` Row |
| [A.5.](./show__vat) | [Vat](./show__vat) | :show__vat | `true` | [A](show__vat#example-a), [B](show__vat#example-b) | Show or Hide `VAT` Row |
| [A.6.](./show__total_gross) | [Total Gross](./show__total_gross) | :show__total_gross | `true` | [A](show__total_gross#example-a), [B](show__total_gross#example-b) | Show or Hide `Total Gross` Row |
| [A.7.](./show__logo) | [Logo](./show__logo) | :show__logo | `false` | [A](show__logo#example-a) | Show or Hide Logo. To set your Image path or base64 string visit [headline__image__src](../options/headline__image__src.html) |
| [A.8.](./show__watermark) | [Watermark](./show__watermark) | :show__watermark | `true` | [A](show__watermark#example-a), [B](show__watermark#example-b) | Show or Hide Watermark. To set watermark text visit [text__watermark](../options/text__watermark)  |
| [A.9.](./show__unencrypted) | [Unencrypted](./show__unencrypted) | :show__unencrypted | `true` |  | Encrypt or unencrypt .pdf document. To set a password visit [Payload](../payload/#example) #example > document > encrypted |


### Order

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [B.1.](./order) | [](./order) | :order | `[{:name=>:header, :move_down=>[0]}, {:name=>:two, :move_down=>[:style__sections__pad]}, {:name=>:three, :move_down=>[:style__sections__pad]}, {:name=>:four, :move_down=>[:style__sections__pad, :style__sections__pad]}, {:name=>:five, :move_down=>[:style__sections__pad, :style__sections__pad]}, {:name=>:six, :move_down=>[0]}, {:name=>:seven, :move_down=>[:style__sections__pad, :style__sections__pad]}, {:name=>:eight, :move_down=>[:style__sections__pad]}]` | [A](order#example-a), [B](order#example-b) | Arrange Sections here. For more Informations see [Sections](../sections/) |


### Text

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [C.1.](./text__phone) | [Phone](./text__phone) | :text__phone | `"Phone:"` | [A](text__phone#example-a), [B](text__phone#example-b) | Set default text `Phone`. Note: Optional you can use Inline Formating. |
| [C.2.](./text__mobile) | [Mobile](./text__mobile) | :text__mobile | `"Mobil:"` | [A](text__mobile#example-a), [B](text__mobile#example-b) | Set default text `Mobile`. Note: Optional you can use Inline Formating. |
| [C.3.](./text__email) | [Email](./text__email) | :text__email | `"Email:"` | [A](text__email#example-a), [B](text__email#example-b) | Set default text `Email`. Note: Optional you can use Inline Formating. |
| [C.4.](./text__website) | [Website](./text__website) | :text__website | `"Website:"` | [A](text__website#example-a), [B](text__website#example-b) | Set default text `Website`. Note: Optional you can use Inline Formating. |
| [C.5.](./text__tax_id) | [Tax Id](./text__tax_id) | :text__tax_id | `"Tax ID:"` | [A](text__tax_id#example-a), [B](text__tax_id#example-b) | Set default text `Tax ID`. Note: Optional you can use Inline Formating. |
| [C.6.](./text__invoice) | [Invoice](./text__invoice) | :text__invoice | `"Invoice"` | [A](text__invoice#example-a), [B](text__invoice#example-b) | Set default text `Invoice`. Note: Optional you can use Inline Formating. |
| [C.7.](./text__page_count) | [Page Count](./text__page_count) | :text__page_count | `"<page> / <total>"` | [A](text__page_count#example-a), [B](text__page_count#example-b) | Set Page count output here. Use `<page>` to show current page number and `<total>` to show sum of all pages. |
| [C.8.](./text__articles__nr) | [Articles Nr](./text__articles__nr) | :text__articles__nr | `"<b>NR</b>"` | [A](text__articles__nr#example-a), [B](text__articles__nr#example-b) | Set Headline Column `"Nr"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.9.](./text__articles__id) | [Articles Id](./text__articles__id) | :text__articles__id | `"<b>ID</b>"` | [A](text__articles__id#example-a), [B](text__articles__id#example-b) | Set Headline Column `"ID"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.10.](./text__articles__article) | [Articles Article](./text__articles__article) | :text__articles__article | `"<b>ARTICLE</b>"` | [A](text__articles__article#example-a), [B](text__articles__article#example-b) | Set Headline Column `"Article"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.11.](./text__articles__piece) | [Articles Piece](./text__articles__piece) | :text__articles__piece | `"<b>PIECE</b>"` | [A](text__articles__piece#example-a), [B](text__articles__piece#example-b) | Set Headline Column `"Piece"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.12.](./text__articles__single) | [Articles Single](./text__articles__single) | :text__articles__single | `"<b>SINGLE</b>"` | [A](text__articles__single#example-a), [B](text__articles__single#example-b) | Set Headline Column `"Single"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.13.](./text__articles__total) | [Articles Total](./text__articles__total) | :text__articles__total | `"<b>TOTAL</b>"` | [A](text__articles__total#example-a), [B](text__articles__total#example-b) | Set Headline Column `"Total"` of Article Section in your preferred Language. Optional you can use Inline Formating. |
| [C.14.](./text__total__sub_total) | [Total Sub Total](./text__total__sub_total) | :text__total__sub_total | `"Subtotal:"` | [A](text__total__sub_total#example-a), [B](text__total__sub_total#example-b) | Set Row `"Sub Total"` in the "Article" Section. For hiding the row see [show__sub_total](../options/show__sub_total) |
| [C.15.](./text__total__shipping) | [Total Shipping](./text__total__shipping) | :text__total__shipping | `"+ Shipping"` | [A](text__total__shipping#example-a), [B](text__total__shipping#example-b) | Set Row `"Total Shipping"` in the "Article" Section. For hiding the row see [show__shipping](../options/show__shipping) |
| [C.16.](./text__total__total_net) | [Total Total Net](./text__total__total_net) | :text__total__total_net | `"<b>Total (net):</b>"` | [A](text__total__total_net#example-a), [B](text__total__total_net#example-b) | Set Row `"Total Net"` in the "Article" Section. For hiding the row see [show__total_net](../options/show__total_net) |
| [C.17.](./text__total__vat) | [Total Vat](./text__total__vat) | :text__total__vat | `"+ VAT 19 %"` | [A](text__total__vat#example-a), [B](text__total__vat#example-b) | Set Row `"Total Vat"` in the "Article" Section. For hiding the row see [show__total_vat](../options/show__total_vat) |
| [C.18.](./text__total__total_gross) | [Total Total Gross](./text__total__total_gross) | :text__total__total_gross | `"<b>Total (gross):</b>"` | [A](text__total__total_gross#example-a), [B](text__total__total_gross#example-b) | Set Row `"Total Gross"` in the "Article" Section. For hiding the row see [show__total_gross](../options/show__total_gross) |
| [C.19.](./text__footer__left) | [Footer Left](./text__footer__left) | :text__footer__left | `"Postal"` | [A](text__footer__left#example-a), [B](text__footer__left#example-b) | Set the `Headline` of Footer on the `Left` column |
| [C.20.](./text__footer__center) | [Footer Center](./text__footer__center) | :text__footer__center | `"Bank"` | [A](text__footer__center#example-a), [B](text__footer__center#example-b) | Set the `Headline` of Footer on the `Center` column. |
| [C.21.](./text__footer__right) | [Footer Right](./text__footer__right) | :text__footer__right | `"Contact"` | [A](text__footer__right#example-a), [B](text__footer__right#example-b) | Set the `Headline` of Footer on the `Right` column. |
| [C.22.](./text__watermark) | [Watermark](./text__watermark) | :text__watermark | `"Example"` | [A](text__watermark#example-a), [B](text__watermark#example-b) | Set `watermark text` |


### Style

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [D.1.](./style__document__format) | [Document Format](./style__document__format) | :style__document__format | `"A4"` | [A](style__document__format#example-a), [B](style__document__format#example-b) | Set Format of the Document here. For more Information visit: [prawnpdf.org/docs/0.11.1/Prawn/Document/PageGeometry.html](https://prawnpdf.org/docs/0.11.1/Prawn/Document/PageGeometry.html) |
| [D.2.](./style__page_count__align) | [Page Count Align](./style__page_count__align) | :style__page_count__align | `:right` | [A](style__page_count__align#example-a), [B](style__page_count__align#example-b) | Set Page Count alignment |
| [D.3.](./style__page_count__start_count_at) | [Page Count Start Count At](./style__page_count__start_count_at) | :style__page_count__start_count_at | `1` | [A](style__page_count__start_count_at#example-a), [B](style__page_count__start_count_at#example-b) | Start to count from. |
| [D.4.](./style__page_count__offset_y) | [Page Count Offset Y](./style__page_count__offset_y) | :style__page_count__offset_y | `0` | [A](style__page_count__offset_y#example-a), [B](style__page_count__offset_y#example-b) | Set an `y offset` for page count string. |
| [D.5.](./style__font__name) | [Font Name](./style__font__name) | :style__font__name | `"Helvetica"` | [A](style__font__name#example-a) | Set standard `font name`. |
| [D.6.](./style__font__family) | [Font Family](./style__font__family) | :style__font__family | `{}` | [A](style__font__family#example-a) | Set standard `font name`. |
| [D.7.](./style__font__default) | [Font Default](./style__font__default) | :style__font__default | `10` | [A](style__font__default#example-a), [B](style__font__default#example-b) | Set default `font size`. |
| [D.8.](./style__font__small) | [Font Small](./style__font__small) | :style__font__small | `8` | [A](style__font__small#example-a), [B](style__font__small#example-b) | Set small `font size`. |
| [D.9.](./style__colors__background) | [Colors Background](./style__colors__background) | :style__colors__background | `"FFFFFF"` | [A](style__colors__background#example-a), [B](style__colors__background#example-b) | Set document background color (not full supported). |
| [D.10.](./style__colors__header__default) | [Colors Header Default](./style__colors__header__default) | :style__colors__header__default | `"000000"` | [A](style__colors__header__default#example-a), [B](style__colors__header__default#example-b) | Set background color for header section |
| [D.11.](./style__colors__rows__even) | [Colors Rows Even](./style__colors__rows__even) | :style__colors__rows__even | `"F0F0F0"` | [A](style__colors__rows__even#example-a), [B](style__colors__rows__even#example-b) | Set color for `even rows` in the article section. |
| [D.12.](./style__colors__rows__odd) | [Colors Rows Odd](./style__colors__rows__odd) | :style__colors__rows__odd | `"FFFFFF"` | [A](style__colors__rows__odd#example-a), [B](style__colors__rows__odd#example-b) | Set color for `even rows` in the article section. |
| [D.13.](./style__header__height) | [Header Height](./style__header__height) | :style__header__height | `90` | [A](style__header__height#example-a), [B](style__header__height#example-b) | Set total height of header section. |
| [D.14.](./style__address_label__offset_x) | [Address Label Offset X](./style__address_label__offset_x) | :style__address_label__offset_x | `20` | [A](style__address_label__offset_x#example-a), [B](style__address_label__offset_x#example-b) | Set `x offset` for address label to adjust position for envelopes with window. |
| [D.15.](./style__address_label__move_down_one) | [Address Label Move Down One](./style__address_label__move_down_one) | :style__address_label__move_down_one | `15` | [A](style__address_label__move_down_one#example-a), [B](style__address_label__move_down_one#example-b) | Set distance between sender and receiver. |
| [D.16.](./style__address_label__move_down_two) | [Address Label Move Down Two](./style__address_label__move_down_two) | :style__address_label__move_down_two | `100` | [A](style__address_label__move_down_two#example-a), [B](style__address_label__move_down_two#example-b) | Set distance between address label and next section. |
| [D.17.](./style__footer__height) | [Footer Height](./style__footer__height) | :style__footer__height | `60` | [A](style__footer__height#example-a), [B](style__footer__height#example-b) | Set total height of footer section. |
| [D.18.](./style__footer__border_width) | [Footer Border Width](./style__footer__border_width) | :style__footer__border_width | `1` | [A](style__footer__border_width#example-a), [B](style__footer__border_width#example-b) | Set border width which differs footer and section before. |
| [D.19.](./style__footer__borders) | [Footer Borders](./style__footer__borders) | :style__footer__borders | `[:top]` | [A](style__footer__borders#example-a), [B](style__footer__borders#example-b) | Set border type which differs footer and section before. |
| [D.20.](./style__sections__pad) | [Sections Pad](./style__sections__pad) | :style__sections__pad | `10` | [A](style__sections__pad#example-a), [B](style__sections__pad#example-b) | Set default padding between sections. |
| [D.21.](./style__articles__nr__align) | [Articles Nr Align](./style__articles__nr__align) | :style__articles__nr__align | `:left` | [A](style__articles__nr__align#example-a), [B](style__articles__nr__align#example-b) | Set align of Article `"Nr"` column. |
| [D.22.](./style__articles__nr__width) | [Articles Nr Width](./style__articles__nr__width) | :style__articles__nr__width | `40` | [A](style__articles__nr__width#example-a), [B](style__articles__nr__width#example-b) | Set width of Article `"Nr"` column. |
| [D.23.](./style__articles__id__align) | [Articles Id Align](./style__articles__id__align) | :style__articles__id__align | `:left` | [A](style__articles__id__align#example-a), [B](style__articles__id__align#example-b) | Set alignment of Article `"ID"` column. |
| [D.24.](./style__articles__id__width) | [Articles Id Width](./style__articles__id__width) | :style__articles__id__width | `60` | [A](style__articles__id__width#example-a), [B](style__articles__id__width#example-b) | Set width of Article `"ID"` column. |
| [D.25.](./style__articles__article__align) | [Articles Article Align](./style__articles__article__align) | :style__articles__article__align | `:left` | [A](style__articles__article__align#example-a), [B](style__articles__article__align#example-b) | Set alignment of Article `"Article"` column. |
| [D.26.](./style__articles__article__width) | [Articles Article Width](./style__articles__article__width) | :style__articles__article__width | `220` | [A](style__articles__article__width#example-a), [B](style__articles__article__width#example-b) | Set width of Article `"Article"` column. |
| [D.27.](./style__articles__piece__align) | [Articles Piece Align](./style__articles__piece__align) | :style__articles__piece__align | `:right` | [A](style__articles__piece__align#example-a), [B](style__articles__piece__align#example-b) | Set alignment of Article `"Piece"` column. |
| [D.28.](./style__articles__piece__width) | [Articles Piece Width](./style__articles__piece__width) | :style__articles__piece__width | `80` | [A](style__articles__piece__width#example-a), [B](style__articles__piece__width#example-b) | Set width of Article `"Piece"` column. |
| [D.29.](./style__articles__single__align) | [Articles Single Align](./style__articles__single__align) | :style__articles__single__align | `:right` | [A](style__articles__single__align#example-a), [B](style__articles__single__align#example-b) | Set alignment of Article `"Single"` column. |
| [D.30.](./style__articles__single__width) | [Articles Single Width](./style__articles__single__width) | :style__articles__single__width | `60` | [A](style__articles__single__width#example-a), [B](style__articles__single__width#example-b) | Set width of Article `"Single"` column. |
| [D.31.](./style__articles__single__format) | [Articles Single Format](./style__articles__single__format) | :style__articles__single__format | `:format_types__currency__short` | [A](style__articles__single__format#example-a) | Set Format Type of Article `"Single"` column. |
| [D.32.](./style__articles__total__align) | [Articles Total Align](./style__articles__total__align) | :style__articles__total__align | `:right` | [A](style__articles__total__align#example-a), [B](style__articles__total__align#example-b) | Set alignement of Article `"Total"` column. |
| [D.33.](./style__articles__total__width) | [Articles Total Width](./style__articles__total__width) | :style__articles__total__width | `60` | [A](style__articles__total__width#example-a), [B](style__articles__total__width#example-b) | Set width of Article `"Total"` column. |
| [D.34.](./style__articles__total__format) | [Articles Total Format](./style__articles__total__format) | :style__articles__total__format | `:format_types__currency__short` | [A](style__articles__total__format#example-a) | Set Format Type of Article `"Total"` column. |
| [D.35.](./style__total__sub_total__borders) | [Total Sub Total Borders](./style__total__sub_total__borders) | :style__total__sub_total__borders | `[:top]` | [A](style__total__sub_total__borders#example-a), [B](style__total__sub_total__borders#example-b) | Set border type of `"Sub Total"` Area in "Article" Section. |
| [D.36.](./style__total__sub_total__border_width) | [Total Sub Total Border Width](./style__total__sub_total__border_width) | :style__total__sub_total__border_width | `1` | [A](style__total__sub_total__border_width#example-a), [B](style__total__sub_total__border_width#example-b) | Set border width of `"Sub Total"` Area in "Article" Section. |
| [D.37.](./style__total__shipping__borders) | [Total Shipping Borders](./style__total__shipping__borders) | :style__total__shipping__borders | `[:top]` | [A](style__total__shipping__borders#example-a), [B](style__total__shipping__borders#example-b) | Set border type of `"Shipping"` Area in "Article" Section. |
| [D.38.](./style__total__shipping__border_width) | [Total Shipping Border Width](./style__total__shipping__border_width) | :style__total__shipping__border_width | `0` | [A](style__total__shipping__border_width#example-a), [B](style__total__shipping__border_width#example-b) | Set border width of `"Shipping"` Area in "Article" Section. |
| [D.39.](./style__total__total_net__borders) | [Total Total Net Borders](./style__total__total_net__borders) | :style__total__total_net__borders | `[:top]` | [A](style__total__total_net__borders#example-a), [B](style__total__total_net__borders#example-b) | Set border type of `"Total Net"` Area in "Article" Section. |
| [D.40.](./style__total__total_net__border_width) | [Total Total Net Border Width](./style__total__total_net__border_width) | :style__total__total_net__border_width | `1` | [A](style__total__total_net__border_width#example-a), [B](style__total__total_net__border_width#example-b) | Set border type of `"Total Net"` Area in "Article" Section. |
| [D.41.](./style__total__vat__borders) | [Total Vat Borders](./style__total__vat__borders) | :style__total__vat__borders | `[:top]` | [A](style__total__vat__borders#example-a), [B](style__total__vat__borders#example-b) | Set border type of `"VAT"` Area in "Article" Section. |
| [D.42.](./style__total__vat__border_width) | [Total Vat Border Width](./style__total__vat__border_width) | :style__total__vat__border_width | `0` | [A](style__total__vat__border_width#example-a), [B](style__total__vat__border_width#example-b) | Set border width of `"VAT"` Area in "Article" Section. |
| [D.43.](./style__total__total_gross__borders) | [Total Total Gross Borders](./style__total__total_gross__borders) | :style__total__total_gross__borders | `[:top]` | [A](style__total__total_gross__borders#example-a), [B](style__total__total_gross__borders#example-b) | Set border type of `"Total Gross"` Area in "Article" Section. |
| [D.44.](./style__total__total_gross__border_width) | [Total Total Gross Border Width](./style__total__total_gross__border_width) | :style__total__total_gross__border_width | `0` | [A](style__total__total_gross__border_width#example-a), [B](style__total__total_gross__border_width#example-b) | Set border width of `"Total Gross"` Area in "Article" Section. |
| [D.45.](./style__qr_code__width) | [Qr Code Width](./style__qr_code__width) | :style__qr_code__width | `40` | [A](style__qr_code__width#example-a), [B](style__qr_code__width#example-b) | Set `QR Code` width (and height). |
| [D.46.](./style__watermark__rotate) | [Watermark Rotate](./style__watermark__rotate) | :style__watermark__rotate | `45` | [A](style__watermark__rotate#example-a), [B](style__watermark__rotate#example-b) | Set `rotation of watermark`. |
| [D.47.](./style__watermark__fill_color) | [Watermark Fill Color](./style__watermark__fill_color) | :style__watermark__fill_color | `"383838"` | [A](style__watermark__fill_color#example-a), [B](style__watermark__fill_color#example-b) | Set `rotation of watermark`. |
| [D.48.](./style__watermark__font_size) | [Watermark Font Size](./style__watermark__font_size) | :style__watermark__font_size | `180` | [A](style__watermark__font_size#example-a), [B](style__watermark__font_size#example-b) | Set `font size` of watermark. |
| [D.49.](./style__watermark__font_family) | [Watermark Font Family](./style__watermark__font_family) | :style__watermark__font_family | `"Times-Roman"` | [A](style__watermark__font_family#example-a), [B](style__watermark__font_family#example-b) | Set `font family`. |
| [D.50.](./style__watermark__transparency) | [Watermark Transparency](./style__watermark__transparency) | :style__watermark__transparency | `0.1` | [A](style__watermark__transparency#example-a), [B](style__watermark__transparency#example-b) | Set watermark `transparency`. |


### Format_types

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [E.1.](./format_types__currency__short) | [Currency Short](./format_types__currency__short) | :format_types__currency__short | `{:delimiter=>".", :separator=>",", :precision=>2, :unit=>"", :format=>"%n €"}` | [A](format_types__currency__short#example-a), [B](format_types__currency__short#example-b) | Define Format Type for viewing currency values in a `short form`. |
| [E.2.](./format_types__currency__long) | [Currency Long](./format_types__currency__long) | :format_types__currency__long | `{:delimiter=>".", :separator=>",", :precision=>2, :unit=>"", :format=>"%n EUR"}` | [A](format_types__currency__long#example-a), [B](format_types__currency__long#example-b) | Define Format Type for viewing currency values in a `long form`. |
| [E.3.](./format_types__date__eu) | [Date Eu](./format_types__date__eu) | :format_types__date__eu | `{:strf=>"%d.%m.%Y"}` | [A](format_types__date__eu#example-a), [B](format_types__date__eu#example-b) | Define Format Type for viewing date values for the `EU region`. |
| [E.4.](./format_types__date__short) | [Date Short](./format_types__date__short) | :format_types__date__short | `{:strf=>"%B %d"}` |  | Define Format Type for viewing date values in a `short form`. (As default not in use) |
| [E.5.](./format_types__date__default) | [Date Default](./format_types__date__default) | :format_types__date__default | `{:strf=>"%B %d, %Y"}` | [A](format_types__date__default#example-a), [B](format_types__date__default#example-b) | Define Format Type for viewing date values by `default`. |
| [E.6.](./format_types__date__long) | [Date Long](./format_types__date__long) | :format_types__date__long | `{:strf=>"%A %B %d %Y %I:%M%P UTC"}` | [A](format_types__date__long#example-a), [B](format_types__date__long#example-b) | Define Format Type for viewing date values in a `long form`. |
| [E.7.](./format_types__date__year) | [Date Year](./format_types__date__year) | :format_types__date__year | `{:strf=>"%Y"}` |  | Define Format Type for showing `only the year`. (As default not in use) |


### Sections

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [F.1.](./sections__nine__left_headline) | [Nine Left Headline](./sections__nine__left_headline) | :sections__nine__left_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__left, :format=>nil}]}` | [A](sections__nine__left_headline#example-a), [B](sections__nine__left_headline#example-b) | Set Headline of the `left footer` column. |
| [F.2.](./sections__nine__left_one) | [Nine Left One](./sections__nine__left_one) | :sections__nine__left_one | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}]}` | [A](sections__nine__left_one#example-a), [B](sections__nine__left_one#example-b) | Set the `first row` of the left footer column. |
| [F.3.](./sections__nine__left_two) | [Nine Left Two](./sections__nine__left_two) | :sections__nine__left_two | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__street, :format=>nil}]}` | [A](sections__nine__left_two#example-a), [B](sections__nine__left_two#example-b) | Set the `second row` of the left footer column. |
| [F.4.](./sections__nine__left_three) | [Nine Left Three](./sections__nine__left_three) | :sections__nine__left_three | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__city, :format=>nil}]}` | [A](sections__nine__left_three#example-a), [B](sections__nine__left_three#example-b) | Set the `third row` of the left footer column. |
| [F.5.](./sections__nine__left_four) | [Nine Left Four](./sections__nine__left_four) | :sections__nine__left_four | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__country, :format=>nil}]}` | [A](sections__nine__left_four#example-a), [B](sections__nine__left_four#example-b) | Set the `fourth row` of the left footer column. |
| [F.6.](./sections__nine__center_headline) | [Nine Center Headline](./sections__nine__center_headline) | :sections__nine__center_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__center, :format=>nil}]}` | [A](sections__nine__center_headline#example-a), [B](sections__nine__center_headline#example-b) | Set Headline of the `center footer column`. |
| [F.7.](./sections__nine__center_one) | [Nine Center One](./sections__nine__center_one) | :sections__nine__center_one | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__name, :format=>nil}]}` | [A](sections__nine__center_one#example-a), [B](sections__nine__center_one#example-b) | Set the `first row` of the center footer column. |
| [F.8.](./sections__nine__center_two) | [Nine Center Two](./sections__nine__center_two) | :sections__nine__center_two | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__iban, :format=>nil}]}` | [A](sections__nine__center_two#example-a), [B](sections__nine__center_two#example-b) | Set the `second row` of the center footer column. |
| [F.9.](./sections__nine__center_three) | [Nine Center Three](./sections__nine__center_three) | :sections__nine__center_three | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__bic, :format=>nil}]}` | [A](sections__nine__center_three#example-a), [B](sections__nine__center_three#example-b) | Set the `third row` of the center footer column. |
| [F.10.](./sections__nine__center_four) | [Nine Center Four](./sections__nine__center_four) | :sections__nine__center_four | `{:content=>nil, :struct=>"<b><<--a-->> <<--b-->></b>", :assigns=>[{:value=>:obj__text__tax_id, :format=>nil}, {:value=>:payload__from__tax_id, :format=>nil}]}` | [A](sections__nine__center_four#example-a), [B](sections__nine__center_four#example-b) | Set the `fourth row` of the center footer column. |
| [F.11.](./sections__nine__right_headline) | [Nine Right Headline](./sections__nine__right_headline) | :sections__nine__right_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__right, :format=>nil}]}` | [A](sections__nine__right_headline#example-a), [B](sections__nine__right_headline#example-b) | Set Headline of the right footer column. |
| [F.12.](./sections__nine__right_one) | [Nine Right One](./sections__nine__right_one) | :sections__nine__right_one | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__phone, :format=>nil}, {:value=>:payload__from__contact__phone, :format=>nil}]}` | [A](sections__nine__right_one#example-a), [B](sections__nine__right_one#example-b) | Set the `first row` of the right footer column. |
| [F.13.](./sections__nine__right_two) | [Nine Right Two](./sections__nine__right_two) | :sections__nine__right_two | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__mobile, :format=>nil}, {:value=>:payload__from__contact__mobile, :format=>nil}]}` | [A](sections__nine__right_two#example-a), [B](sections__nine__right_two#example-b) | Set the second row of the right footer column. |
| [F.14.](./sections__nine__right_three) | [Nine Right Three](./sections__nine__right_three) | :sections__nine__right_three | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__email, :format=>nil}, {:value=>:payload__from__contact__email, :format=>nil}]}` | [A](sections__nine__right_three#example-a), [B](sections__nine__right_three#example-b) | Set the `third row` of the right footer column. |
| [F.15.](./sections__nine__right_four) | [Nine Right Four](./sections__nine__right_four) | :sections__nine__right_four | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__website, :format=>nil}, {:value=>:payload__from__contact__website, :format=>nil}]}` | [A](sections__nine__right_four#example-a), [B](sections__nine__right_four#example-b) | Set the `fourth row` of the right footer column. |
| [F.16.](./sections__eight__snippet) | [Eight Snippet](./sections__eight__snippet) | :sections__eight__snippet | `{:content=>nil, :struct=>"Thank you for using <<--a-->> Services.\n\n\nSincerely,\n\n<<--a-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}]}` | [A](sections__eight__snippet#example-a), [B](sections__eight__snippet#example-b) | Define text for section eight. |
| [F.17.](./sections__seven__snippet) | [Seven Snippet](./sections__seven__snippet) | :sections__seven__snippet | `{:content=>nil, :struct=>" We will debit your bank account for <b><<--a-->></b> on <<--b-->>. Please ensure you have sufficient funds in your bank account to avoid service disruptions.", :assigns=>[{:value=>:payload__items__total_gross, :format=>:obj__format_types__currency__long}, {:value=>:payload__date__billing, :format=>:obj__format_types__date__long}]}` | [A](sections__seven__snippet#example-a), [B](sections__seven__snippet#example-b) | Define text for section `seven`. |
| [F.18.](./sections__six__sub_total) | [Six Sub Total](./sections__six__sub_total) | :sections__six__sub_total | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__items__sub_total, :format=>:obj__format_types__currency__short}]}` | [A](sections__six__sub_total#example-a), [B](sections__six__sub_total#example-b) | Define text for area `"Sub Total"` in section "six". |
| [F.19.](./sections__six__shipping) | [Six Shipping](./sections__six__shipping) | :sections__six__shipping | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__items__shipping_fee, :format=>:obj__format_types__currency__short}]}` | [A](sections__six__shipping#example-a), [B](sections__six__shipping#example-b) | Define text for area `"Shipping"` in section "six". |
| [F.20.](./sections__six__total_net) | [Six Total Net](./sections__six__total_net) | :sections__six__total_net | `{:content=>nil, :struct=>"<b><<--a-->><b> ", :assigns=>[{:value=>:payload__items__total_net, :format=>:obj__format_types__currency__short}]}` | [A](sections__six__total_net#example-a), [B](sections__six__total_net#example-b) | Define text for area `"Total Net"` in section "six". |
| [F.21.](./sections__six__vat) | [Six Vat](./sections__six__vat) | :sections__six__vat | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__items__vat, :format=>:obj__format_types__currency__short}]}` | [A](sections__six__vat#example-a), [B](sections__six__vat#example-b) | Define text for area `"Vat"` in section "six". |
| [F.22.](./sections__six__total_gross) | [Six Total Gross](./sections__six__total_gross) | :sections__six__total_gross | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:payload__items__total_gross, :format=>:obj__format_types__currency__short}]}` | [A](sections__six__total_gross#example-a), [B](sections__six__total_gross#example-b) | Define text for area `"Total Gross"` in section "six". |
| [F.23.](./sections__four__snippet) | [Four Snippet](./sections__four__snippet) | :sections__four__snippet | `{:content=>nil, :struct=>"Greetings from <<--a-->>,\n\nThis is a <u>demo invoice</u> for usage of <<--a-->> services for billing period <b><<--b-->> - <<--c-->></b>.", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__date__period__from, :format=>:obj__format_types__date__short}, {:value=>:payload__date__period__to, :format=>:obj__format_types__date__default}]}` | [A](sections__four__snippet#example-a), [B](sections__four__snippet#example-b) | Define text for section "four". |
| [F.24.](./sections__three__qr_code) | [Three Qr Code](./sections__three__qr_code) | :sections__three__qr_code | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__meta__qr_code, :format=>nil}]}` | [A](sections__three__qr_code#example-a), [B](sections__three__qr_code#example-b) | Define text for `"QR Code"` in section "three". |
| [F.25.](./sections__three__date) | [Three Date](./sections__three__date) | :sections__three__date | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__date__invoice, :format=>:obj__format_types__date__eu}]}` | [A](sections__three__date#example-a), [B](sections__three__date#example-b) | Define `date` in section "three" |
| [F.26.](./sections__three__headline) | [Three Headline](./sections__three__headline) | :sections__three__headline | `{:content=>nil, :struct=>"<b><<--a-->> | <<--b-->></b>", :assigns=>[{:value=>:obj__text__invoice, :format=>nil}, {:value=>:payload__meta__id, :format=>nil}]}` | [A](sections__three__headline#example-a), [B](sections__three__headline#example-b) | Define `headlinev in section "three". |
| [F.27.](./sections__two__small) | [Two Small](./sections__two__small) | :sections__two__small | `{:content=>nil, :struct=>"<u><<--a-->> - <<--b-->> - <<--c-->></u>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__from__address__street, :format=>nil}, {:value=>:payload__from__address__city, :format=>nil}]}` | [A](sections__two__small#example-a), [B](sections__two__small#example-b) | Define address label (from) in section "two" |


### Headline

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [G.1.](./headline__grid__x) | [Grid X](./headline__grid__x) | :headline__grid__x | `3` |  | Set grid size on the `x axis`. |
| [G.2.](./headline__grid__y) | [Grid Y](./headline__grid__y) | :headline__grid__y | `1` |  | Set grid size on the `y axis`. |
| [G.3.](./headline__default__content) | [Default Content](./headline__default__content) | :headline__default__content | `""` | [A](headline__default__content#example-a), [B](headline__default__content#example-b) | `Autofill` every cell with content if you wish. |
| [G.4.](./headline__default__style) | [Default Style](./headline__default__style) | :headline__default__style | `:style__document__font_size__small` | [A](headline__default__style#example-a), [B](headline__default__style#example-b) | Set `font style` as a reference. |
| [G.5.](./headline__default__align) | [Default Align](./headline__default__align) | :headline__default__align | `:right` | [A](headline__default__align#example-a), [B](headline__default__align#example-b) | Set default aligment behaviour of text. |
| [G.6.](./headline__default__text_color) | [Default Text Color](./headline__default__text_color) | :headline__default__text_color | `:style__colors__header__default` | [A](headline__default__text_color#example-a), [B](headline__default__text_color#example-b) | Set `default text` color in section "one" (headline). |
| [G.7.](./headline__default__borders) | [Default Borders](./headline__default__borders) | :headline__default__borders | `[:left]` | [A](headline__default__borders#example-a), [B](headline__default__borders#example-b) | Set `border type` in section "one" (headline). |
| [G.8.](./headline__default__border_width) | [Default Border Width](./headline__default__border_width) | :headline__default__border_width | `2` | [A](headline__default__border_width#example-a), [B](headline__default__border_width#example-b) | Set `border width` in section "one" (headline). |
| [G.9.](./headline__image__src) | [Image Src](./headline__image__src) | :headline__image__src | `""` | [A](headline__image__src#example-a) | Set local `image path` for company logo, use .png or .jpg |
| [G.10.](./headline__image__colspan) | [Image Colspan](./headline__image__colspan) | :headline__image__colspan | `2` |  | Set how many cells in the `columns (x)` direction should be merge to show the image. |
| [G.11.](./headline__image__rowspan) | [Image Rowspan](./headline__image__rowspan) | :headline__image__rowspan | `2` |  | Set how many cells in the `rows (y)` direction should be merge to show the image. |
| [G.12.](./headline__image__grid) | [Image Grid](./headline__image__grid) | :headline__image__grid | `[0, 0]` |  | Set start position `[ columns x, rows y ]` of image. |
| [G.13.](./headline__image__borders) | [Image Borders](./headline__image__borders) | :headline__image__borders | `[]` |  | Set `border type` of image cell. |
| [G.14.](./headline__image__fit) | [Image Fit](./headline__image__fit) | :headline__image__fit | `[160, 100]` |  | Use `fit size` to adjust the image. |
| [G.15.](./headline__image__border_width) | [Image Border Width](./headline__image__border_width) | :headline__image__border_width | `0` |  | Set `border width` of image cell. |
| [G.16.](./headline__texts) | [Texts](./headline__texts) | :headline__texts | `[{:content=>:sections__one__name__content, :grid=>[2, 0], :style=>:style__document__font_size__h1, :align=>:right, :text_color=>:style__colors__header__default, :borders=>[], :border_width=>0}]` |  | Set a reference to `string data`. |


### Footer

| **Nr** | **Name** | **Key** | **Default** | **Examples** | **Description** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| [H.1.](./footer__left__one) | [Left One](./footer__left__one) | :footer__left__one | `:sections__nine__left_one__content` | [A](footer__left__one#example-a), [B](footer__left__one#example-b) | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.2.](./footer__left__two) | [Left Two](./footer__left__two) | :footer__left__two | `:sections__nine__left_two__content` | [A](footer__left__two#example-a), [B](footer__left__two#example-b) | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.3.](./footer__left__three) | [Left Three](./footer__left__three) | :footer__left__three | `:sections__nine__left_three__content` | [A](footer__left__three#example-a), [B](footer__left__three#example-b) | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.4.](./footer__left__four) | [Left Four](./footer__left__four) | :footer__left__four | `:sections__nine__left_four__content` | [A](footer__left__four#example-a), [B](footer__left__four#example-b) | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.5.](./footer__center__one) | [Center One](./footer__center__one) | :footer__center__one | `:sections__nine__center_one__content` | [A](footer__center__one#example-a), [B](footer__center__one#example-b) | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.6.](./footer__center__two) | [Center Two](./footer__center__two) | :footer__center__two | `:sections__nine__center_two__content` | [A](footer__center__two#example-a), [B](footer__center__two#example-b) | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.7.](./footer__center__three) | [Center Three](./footer__center__three) | :footer__center__three | `:sections__nine__center_three__content` | [A](footer__center__three#example-a), [B](footer__center__three#example-b) | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.8.](./footer__center__four) | [Center Four](./footer__center__four) | :footer__center__four | `:sections__nine__center_four__content` | [A](footer__center__four#example-a), [B](footer__center__four#example-b) | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.9.](./footer__right__one) | [Right One](./footer__right__one) | :footer__right__one | `:sections__nine__right_one__content` | [A](footer__right__one#example-a), [B](footer__right__one#example-b) | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.10.](./footer__right__two) | [Right Two](./footer__right__two) | :footer__right__two | `:sections__nine__right_two__content` | [A](footer__right__two#example-a), [B](footer__right__two#example-b) | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.11.](./footer__right__three) | [Right Three](./footer__right__three) | :footer__right__three | `:sections__nine__right_three__content` | [A](footer__right__three#example-a), [B](footer__right__three#example-b) | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.12.](./footer__right__four) | [Right Four](./footer__right__four) | :footer__right__four | `:sections__nine__right_four__content` | [A](footer__right__four#example-a), [B](footer__right__four#example-b) | Set a reference for `"right"` "footer" section to a formatted string. |