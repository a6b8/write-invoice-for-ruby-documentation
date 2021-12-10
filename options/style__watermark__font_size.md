---
sort: 80
title: D.48 style__watermark__font_size
---
# style__watermark__font_size

Set `font size` of watermark.


## Preview

<div >
    <canvas id='canvas' search=':style__watermark__font_size' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__watermark__font_size => 180
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__watermark__font_size``` |  [Style](./#style) | [All](../sections/) |

### Value

Allow positive integers beginning from 1 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```180``` | ```^[1-9]d*$``` | Integer |

## Example A.

Change `font size` to `40`.

### Output

<img src="../assets/images/options/style__watermark__font_size--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:show__watermark => true, :style__watermark__font_size => 40}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :show__watermark => true, :style__watermark__font_size => 40
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change `font size` to `40`.

### Output

<img src="../assets/images/options/style__watermark__font_size--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:show__watermark => true, :text__watermark => "Demo", :style__watermark__font_size => 200}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :show__watermark => true,
 :text__watermark => "Demo",
 :style__watermark__font_size => 200
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

