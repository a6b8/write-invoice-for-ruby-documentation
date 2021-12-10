---
sort: 2
title: B. Two
---

# Section: Two

The origin position of this section is based below "header" and contains the address field of the receiver.


## Preview

<div >
    <canvas id='canvas' search='two' palette='section_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  
 

## Options

| **Nr** | **Name** | **Key** | **Default** | **Description** |
| :--- | :--- | :--- | :--- | :--- |
| [D.14](/options/#style) | [Style Address Label Offset X](/options/style__address_label__offset_x) | :style__address_label__offset_x | `20` | Set `x offset` for address label to adjust position for envelopes with window. |
| [D.15](/options/#style) | [Style Address Label Move Down One](/options/style__address_label__move_down_one) | :style__address_label__move_down_one | `15` | Set distance between sender and receiver. |
| [D.16](/options/#style) | [Style Address Label Move Down Two](/options/style__address_label__move_down_two) | :style__address_label__move_down_two | `100` | Set distance between address label and next section. |
| [F.27](/options/#sections) | [Sections Two Small](/options/sections__two__small) | :sections__two__small | `{:content=>nil, :struct=>"<u><<--a-->> - <<--b-->> - <<--c-->></u>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__from__address__street, :format=>nil}, {:value=>:payload__from__address__city, :format=>nil}]}` | Define address label (from) in section "two" |
| [F.28](/options/#sections) | [Sections Two To](/options/sections__two__to) | :sections__two__to | `{:content=>nil, :struct=>"\t\t<b><<--a-->></b>\n<<--b-->>\n<<--c-->>\nTax ID: <<--d-->>", :assigns=>[{:value=>:payload__to__address__name, :format=>nil}, {:value=>:payload__to__address__street, :format=>nil}, {:value=>:payload__to__address__city, :format=>nil}, {:value=>:payload__to__tax_id, :format=>nil}]}` | Define address label (to) in section "two" |


