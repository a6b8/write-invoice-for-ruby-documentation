---
sort: 51
title: D.19 style__footer__borders
---
# style__footer__borders

Set border type which differs footer and section before.


## Preview

<div >
    <canvas id='canvas' search=':style__footer__borders' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :style__footer__borders => [:top]
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:style__footer__borders``` |  [Style](./#style) | [Footer](/sections/footer) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```[:top]``` | ```^[a-zA-Z0-9]*$``` | Array |

## Example A.

Change border style to `:left`.

### Output

<img src="../assets/images/options/style__footer__borders--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__footer__borders => [:left]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__footer__borders => [:left]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change border style to `:right` and `:top`.

### Output

<img src="../assets/images/options/style__footer__borders--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:style__footer__borders => [:right, :top]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :style__footer__borders => [:right, :top]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

