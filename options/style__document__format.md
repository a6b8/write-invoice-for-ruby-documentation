---
sort: 33
title: D.1 style__document__format
---
# style__document__format

Set Format of the Document here. For more Information visit: [prawnpdf.org/docs/0.11.1/Prawn/Document/PageGeometry.html](https://prawnpdf.org/docs/0.11.1/Prawn/Document/PageGeometry.html)


## Preview

<div >
    <canvas id='canvas' search=':style__document__format' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__document__format => "A4"
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__document__format``` |  [Style](./#style) | [All](../sections/) |

### Value

Allow A-Z, a-b and 0-9 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```"A4"``` | ```^[a-zA-Z0-9_]*$``` | String |

## Example A.

Set to `"LETTER"`.

### Output

<img src="../assets/images/options/style__document__format--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__document__format => "LETTER"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__document__format => "LETTER"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Set to `"LEGAL"`.

### Output

<img src="../assets/images/options/style__document__format--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__document__format => "LEGAL"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__document__format => "LEGAL"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

