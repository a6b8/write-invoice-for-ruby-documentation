---
sort: 38
title: D.6 style__font__family
---
# style__font__family

Set standard `font name`.


## Preview

<div >
    <canvas id='canvas' search=':style__font__family' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__font__family => {}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__font__family``` |  [Style](./#style) | [All](../sections/) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Set font name to `RanaCom`.

### Output

<img src="../assets/images/options/style__font__family--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__font__name => "RanaCom", :style__font__family =>   {"RanaCom" =>     {:normal => "~/Library/Fonts/RanaCom-Regular.ttf",     :italic => "~/Library/Fonts/RanaCom-Italic.ttf",     :bold => "~/Library/Fonts/RanaCom-Bold.ttf",     :bold_italic => "~/Library/Fonts/RanaCom-BlackItalic.ttf"}}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__font__name => "RanaCom",
 :style__font__family => 
  {"RanaCom" => 
    {:normal => "~/Library/Fonts/RanaCom-Regular.ttf",
     :italic => "~/Library/Fonts/RanaCom-Italic.ttf",
     :bold => "~/Library/Fonts/RanaCom-Bold.ttf",
     :bold_italic => "~/Library/Fonts/RanaCom-BlackItalic.ttf"}}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

