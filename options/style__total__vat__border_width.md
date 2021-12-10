---
sort: 74
title: D.42 style__total__vat__border_width
---
# style__total__vat__border_width

Set border width of `"VAT"` Area in "Article" Section.


## Preview

<div >
    <canvas id='canvas' search=':style__total__vat__border_width' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__total__vat__border_width => 0
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__total__vat__border_width``` |  [Style](./#style) | [Six](/sections/six) |

### Value

Allow positive integers beginning from 1 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```0``` | ```^[1-9]d*$``` | Integer |

## Example A.

Set border width to `4`.

### Output

<img src="../assets/images/options/style__total__vat__border_width--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__total__vat__border_width => 4}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__total__vat__border_width => 4
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Set border width to `10`.

### Output

<img src="../assets/images/options/style__total__vat__border_width--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__total__vat__border_width => 10}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__total__vat__border_width => 10
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

