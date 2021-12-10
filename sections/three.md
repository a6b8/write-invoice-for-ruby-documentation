---
sort: 3
title: C. Three
---

# Section: Three

The origin position of this section is based below address field and contains two text field on the left and a qr code field on the right. 


## Preview

<div >
    <canvas id='canvas' search='three' palette='section_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  
 

## Options

| **Nr** | **Name** | **Key** | **Default** | **Description** |
| :--- | :--- | :--- | :--- | :--- |
| [A.1](/options/#show) | [Show Qr Code](/options/show__qr_code) | :show__qr_code | `true` | Show or Hide `QR Code` Image |
| [C.6](/options/#text) | [Text Invoice](/options/text__invoice) | :text__invoice | `Invoice` | Set default text `Invoice`. Note: Optional you can use Inline Formating. |
| [D.45](/options/#style) | [Style Qr Code Width](/options/style__qr_code__width) | :style__qr_code__width | `40` | Set `QR Code` width (and height). |
| [E.3](/options/#format_types) | [Format Types Date Eu](/options/format_types__date__eu) | :format_types__date__eu | `{:strf=>"%d.%m.%Y"}` | Define Format Type for viewing date values for the `EU region`. |
| [F.24](/options/#sections) | [Sections Three Qr Code](/options/sections__three__qr_code) | :sections__three__qr_code | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__meta__qr_code, :format=>nil}]}` | Define text for `"QR Code"` in section "three". |
| [F.25](/options/#sections) | [Sections Three Date](/options/sections__three__date) | :sections__three__date | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__date__invoice, :format=>:obj__format_types__date__eu}]}` | Define `date` in section "three" |
| [F.26](/options/#sections) | [Sections Three Headline](/options/sections__three__headline) | :sections__three__headline | `{:content=>nil, :struct=>"<b><<--a-->> | <<--b-->></b>", :assigns=>[{:value=>:obj__text__invoice, :format=>nil}, {:value=>:payload__meta__id, :format=>nil}]}` | Define `headlinev in section "three". |


