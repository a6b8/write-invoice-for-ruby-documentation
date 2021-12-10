---
sort: 9
title: I. Footer
---

# Section: Footer

The origin position of this section is based on the bottom as "footer". You have a table with 3 columns and 4 rows to include your data.


## Preview

<div >
    <canvas id='canvas' search='footer' palette='section_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  
 

## Options

| **Nr** | **Name** | **Key** | **Default** | **Description** |
| :--- | :--- | :--- | :--- | :--- |
| [C.1](/options/#text) | [Text Phone](/options/text__phone) | :text__phone | `Phone:` | Set default text `Phone`. Note: Optional you can use Inline Formating. |
| [C.2](/options/#text) | [Text Mobile](/options/text__mobile) | :text__mobile | `Mobil:` | Set default text `Mobile`. Note: Optional you can use Inline Formating. |
| [C.3](/options/#text) | [Text Email](/options/text__email) | :text__email | `Email:` | Set default text `Email`. Note: Optional you can use Inline Formating. |
| [C.4](/options/#text) | [Text Website](/options/text__website) | :text__website | `Website:` | Set default text `Website`. Note: Optional you can use Inline Formating. |
| [C.5](/options/#text) | [Text Tax](/options/text__tax_id) | :text__tax_id | `Tax ID:` | Set default text `Tax ID`. Note: Optional you can use Inline Formating. |
| [C.19](/options/#text) | [Text Footer Left](/options/text__footer__left) | :text__footer__left | `Postal` | Set the `Headline` of Footer on the `Left` column |
| [C.20](/options/#text) | [Text Footer Center](/options/text__footer__center) | :text__footer__center | `Bank` | Set the `Headline` of Footer on the `Center` column. |
| [C.21](/options/#text) | [Text Footer Right](/options/text__footer__right) | :text__footer__right | `Contact` | Set the `Headline` of Footer on the `Right` column. |
| [D.18](/options/#style) | [Style Footer Border Width](/options/style__footer__border_width) | :style__footer__border_width | `1` | Set border width which differs footer and section before. |
| [D.19](/options/#style) | [Style Footer Borders](/options/style__footer__borders) | :style__footer__borders | `[:top]` | Set border type which differs footer and section before. |
| [F.1](/options/#sections) | [Sections Nine Left Headline](/options/sections__nine__left_headline) | :sections__nine__left_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__left, :format=>nil}]}` | Set Headline of the `left footer` column. |
| [F.2](/options/#sections) | [Sections Nine Left One](/options/sections__nine__left_one) | :sections__nine__left_one | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}]}` | Set the `first row` of the left footer column. |
| [F.3](/options/#sections) | [Sections Nine Left Two](/options/sections__nine__left_two) | :sections__nine__left_two | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__street, :format=>nil}]}` | Set the `second row` of the left footer column. |
| [F.4](/options/#sections) | [Sections Nine Left Three](/options/sections__nine__left_three) | :sections__nine__left_three | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__city, :format=>nil}]}` | Set the `third row` of the left footer column. |
| [F.5](/options/#sections) | [Sections Nine Left Four](/options/sections__nine__left_four) | :sections__nine__left_four | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__address__country, :format=>nil}]}` | Set the `fourth row` of the left footer column. |
| [F.6](/options/#sections) | [Sections Nine Center Headline](/options/sections__nine__center_headline) | :sections__nine__center_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__center, :format=>nil}]}` | Set Headline of the `center footer column`. |
| [F.7](/options/#sections) | [Sections Nine Center One](/options/sections__nine__center_one) | :sections__nine__center_one | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__name, :format=>nil}]}` | Set the `first row` of the center footer column. |
| [F.8](/options/#sections) | [Sections Nine Center Two](/options/sections__nine__center_two) | :sections__nine__center_two | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__iban, :format=>nil}]}` | Set the `second row` of the center footer column. |
| [F.9](/options/#sections) | [Sections Nine Center Three](/options/sections__nine__center_three) | :sections__nine__center_three | `{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__from__bank__bic, :format=>nil}]}` | Set the `third row` of the center footer column. |
| [F.10](/options/#sections) | [Sections Nine Center Four](/options/sections__nine__center_four) | :sections__nine__center_four | `{:content=>nil, :struct=>"<b><<--a-->> <<--b-->></b>", :assigns=>[{:value=>:obj__text__tax_id, :format=>nil}, {:value=>:payload__from__tax_id, :format=>nil}]}` | Set the `fourth row` of the center footer column. |
| [F.11](/options/#sections) | [Sections Nine Right Headline](/options/sections__nine__right_headline) | :sections__nine__right_headline | `{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__right, :format=>nil}]}` | Set Headline of the right footer column. |
| [F.12](/options/#sections) | [Sections Nine Right One](/options/sections__nine__right_one) | :sections__nine__right_one | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__phone, :format=>nil}, {:value=>:payload__from__contact__phone, :format=>nil}]}` | Set the `first row` of the right footer column. |
| [F.13](/options/#sections) | [Sections Nine Right Two](/options/sections__nine__right_two) | :sections__nine__right_two | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__mobile, :format=>nil}, {:value=>:payload__from__contact__mobile, :format=>nil}]}` | Set the second row of the right footer column. |
| [F.14](/options/#sections) | [Sections Nine Right Three](/options/sections__nine__right_three) | :sections__nine__right_three | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__email, :format=>nil}, {:value=>:payload__from__contact__email, :format=>nil}]}` | Set the `third row` of the right footer column. |
| [F.15](/options/#sections) | [Sections Nine Right Four](/options/sections__nine__right_four) | :sections__nine__right_four | `{:content=>nil, :struct=>"<<--a-->> <<--b-->>", :assigns=>[{:value=>:obj__text__website, :format=>nil}, {:value=>:payload__from__contact__website, :format=>nil}]}` | Set the `fourth row` of the right footer column. |
| [H.1](/options/#footer) | [Footer Left One](/options/footer__left__one) | :footer__left__one | `sections__nine__left_one__content` | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.2](/options/#footer) | [Footer Left Two](/options/footer__left__two) | :footer__left__two | `sections__nine__left_two__content` | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.3](/options/#footer) | [Footer Left Three](/options/footer__left__three) | :footer__left__three | `sections__nine__left_three__content` | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.4](/options/#footer) | [Footer Left Four](/options/footer__left__four) | :footer__left__four | `sections__nine__left_four__content` | Set a reference for `"left"` "footer" section to a formatted string. |
| [H.5](/options/#footer) | [Footer Center One](/options/footer__center__one) | :footer__center__one | `sections__nine__center_one__content` | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.6](/options/#footer) | [Footer Center Two](/options/footer__center__two) | :footer__center__two | `sections__nine__center_two__content` | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.7](/options/#footer) | [Footer Center Three](/options/footer__center__three) | :footer__center__three | `sections__nine__center_three__content` | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.8](/options/#footer) | [Footer Center Four](/options/footer__center__four) | :footer__center__four | `sections__nine__center_four__content` | Set a reference for `"center"` "footer" section to a formatted string. |
| [H.9](/options/#footer) | [Footer Right One](/options/footer__right__one) | :footer__right__one | `sections__nine__right_one__content` | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.10](/options/#footer) | [Footer Right Two](/options/footer__right__two) | :footer__right__two | `sections__nine__right_two__content` | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.11](/options/#footer) | [Footer Right Three](/options/footer__right__three) | :footer__right__three | `sections__nine__right_three__content` | Set a reference for `"right"` "footer" section to a formatted string. |
| [H.12](/options/#footer) | [Footer Right Four](/options/footer__right__four) | :footer__right__four | `sections__nine__right_four__content` | Set a reference for `"right"` "footer" section to a formatted string. |


