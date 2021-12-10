---
sort: 125
title: G.7 headline__default__borders
---
# headline__default__borders

Set `border type` in section "one" (headline).


## Preview

<div >
    <canvas id='canvas' search=':headline__default__borders' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :headline__default__borders => [:left]
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:headline__default__borders``` |  [Headline](./#headline) | [Header](/sections/header) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```[:left]``` | ```^[a-zA-Z0-9]*$``` | Array |

## Example A.

Change headline border type to `:right`.

### Output

<img src="../assets/images/options/headline__default__borders--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:headline__default__borders => [:right]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :headline__default__borders => [:right]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change headline border type to `:left` and `:right`.

### Output

<img src="../assets/images/options/headline__default__borders--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:headline__default__borders => [:left, :right]}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :headline__default__borders => [:left, :right]
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

