---
sort: 44
title: D.12 style__colors__rows__odd
---
# style__colors__rows__odd

Set color for `even rows` in the article section.


## Preview

<div >
    <canvas id='canvas' search=':style__colors__rows__odd' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__colors__rows__odd => "FFFFFF"
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__colors__rows__odd``` |  [Style](./#style) | [Five](/sections/five) |

### Value

Allow A-Z, a-b and 0-9 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```"FFFFFF"``` | ```^[a-zA-Z0-9_]*$``` | String |

## Example A.

Set background color to `#DCDCDC`.

### Output

<img src="../assets/images/options/style__colors__rows__odd--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__colors__rows__odd => "DCDCDC"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__colors__rows__odd => "DCDCDC"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Set default font size to `#9181AD`.

### Output

<img src="../assets/images/options/style__colors__rows__odd--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__colors__rows__odd => "9181AD"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__colors__rows__odd => "9181AD"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

