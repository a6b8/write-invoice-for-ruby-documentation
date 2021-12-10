---
sort: 7
title: G. Seven
---

# Section: Seven

The origin position of this section is based below the two product section and include a text field. 


## Preview

<div >
    <canvas id='canvas' search='seven' palette='section_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  
 

## Options

| **Nr** | **Name** | **Key** | **Default** | **Description** |
| :--- | :--- | :--- | :--- | :--- |
| [E.2](/options/#format_types) | [Format Types Currency Long](/options/format_types__currency__long) | :format_types__currency__long | `{:delimiter=>".", :separator=>",", :precision=>2, :unit=>"", :format=>"%n EUR"}` | Define Format Type for viewing currency values in a `long form`. |
| [F.17](/options/#sections) | [Sections Seven Snippet](/options/sections__seven__snippet) | :sections__seven__snippet | `{:content=>nil, :struct=>" We will debit your bank account for <b><<--a-->></b> on <<--b-->>. Please ensure you have sufficient funds in your bank account to avoid service disruptions.", :assigns=>[{:value=>:payload__items__total_gross, :format=>:obj__format_types__currency__long}, {:value=>:payload__date__billing, :format=>:obj__format_types__date__long}]}` | Define text for section `seven`. |


