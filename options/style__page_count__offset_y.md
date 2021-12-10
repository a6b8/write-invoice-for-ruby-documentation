---
sort: 36
title: D.4 style__page_count__offset_y
---
# style__page_count__offset_y

Set an `y offset` for page count string.


## Preview

<div >
    <canvas id='canvas' search=':style__page_count__offset_y' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__page_count__offset_y => 0
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__page_count__offset_y``` |  [Style](./#style) | [Header](/sections/header) |

### Value

Allow positive integers beginning from 1 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```0``` | ```^[1-9]d*$``` | Integer |

## Example A.

Set to `0`.

### Output

<img src="../assets/images/options/style__page_count__offset_y--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__page_count__offset_y => 0}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__page_count__offset_y => 0
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Set to `50`.

### Output

<img src="../assets/images/options/style__page_count__offset_y--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__page_count__offset_y => 50}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__page_count__offset_y => 50
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

