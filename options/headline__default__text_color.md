---
sort: 124
title: G.6 headline__default__text_color
---
# headline__default__text_color

Set `default text` color in section "one" (headline).


## Preview

<div >
    <canvas id='canvas' search=':headline__default__text_color' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :headline__default__text_color => :style__colors__header__default
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:headline__default__text_color``` |  [Headline](./#headline) | [Header](/sections/header) |

### Value

Allow only Type Symbol

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```:style__colors__header__default``` | ```:^[a-zA-Z0-9_]*$``` | Symbol |

## Example A.

Change color to rows `even` to `:style__colors__rows__even`.

### Output

<img src="../assets/images/options/headline__default__text_color--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:headline__default__text_color => :style__colors__rows__even}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :headline__default__text_color => :style__colors__rows__even
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change color to rows `odd` to `:style__colors__rows__odd`.

### Output

<img src="../assets/images/options/headline__default__text_color--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:headline__default__text_color => :style__colors__rows__odd}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :headline__default__text_color => :style__colors__rows__odd
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

