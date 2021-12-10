---
sort: 71
title: D.39 style__total__total_net__borders
---
# style__total__total_net__borders

Set border type of `"Total Net"` Area in "Article" Section.


## Preview

<div >
    <canvas id='canvas' search=':style__total__total_net__borders' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__total__total_net__borders => [:top]
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__total__total_net__borders``` |  [Style](./#style) | [Six](/sections/six) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```[:top]``` | ```^[a-zA-Z0-9]*$``` | Array |

## Example A.

Set border style to `:bottom`.

### Output

<img src="../assets/images/options/style__total__total_net__borders--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__total__total_net__borders => [:left, :right]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__total__total_net__borders => [:left, :right]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Set border style to `:left`.

### Output

<img src="../assets/images/options/style__total__total_net__borders--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__total__total_net__borders => [:top, :left]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__total__total_net__borders => [:top, :left]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

