---
sort: 78
title: D.46 style__watermark__rotate
---
# style__watermark__rotate

Set `rotation of watermark`.


## Preview

<div >
    <canvas id='canvas' search=':style__watermark__rotate' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__watermark__rotate => 45
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__watermark__rotate``` |  [Style](./#style) | [All](../sections/) |

### Value

Allow positive integers beginning from 1 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```45``` | ```^[1-9]d*$``` | Integer |

## Example A.

Change rotation to `10`

### Output

<img src="../assets/images/options/style__watermark__rotate--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:show__watermark => true, :style__watermark__rotate => 10}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :show__watermark => true, :style__watermark__rotate => 10
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change rotation to `180` and set text to `Confidential` and re-adjust font size.

### Output

<img src="../assets/images/options/style__watermark__rotate--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:show__watermark => true, :text__watermark => "Confidential", :style__watermark__font_size => 180, :style__watermark__rotate => 10}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :show__watermark => true,
 :text__watermark => "Confidential",
 :style__watermark__font_size => 180,
 :style__watermark__rotate => 10
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

