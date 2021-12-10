---
sort: 47
title: D.15 style__address_label__move_down_one
---
# style__address_label__move_down_one

Set distance between sender and receiver.


## Preview

<div >
    <canvas id='canvas' search=':style__address_label__move_down_one' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__address_label__move_down_one => 15
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__address_label__move_down_one``` |  [Style](./#style) | [Two](/sections/two) |

### Value

Allow positive integers beginning from 1 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```15``` | ```^[1-9]d*$``` | Integer |

## Example A.

Move down by `30`.

### Output

<img src="../assets/images/options/style__address_label__move_down_one--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__address_label__move_down_one => 30}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__address_label__move_down_one => 30
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Move down `0`.

### Output

<img src="../assets/images/options/style__address_label__move_down_one--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__address_label__move_down_one => 0}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__address_label__move_down_one => 0
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

