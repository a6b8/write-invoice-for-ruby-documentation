---
sort: 87
title: E.5 format_types__date__default
---
# format_types__date__default

Define Format Type for viewing date values by `default`.


## Preview

<div >
    <canvas id='canvas' search=':format_types__date__default' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :format_types__date__default => {:strf => "%B %d, %Y"}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:format_types__date__default``` |  [Format Types](./#format_types) | [All](../sections/) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:strf=>"%B %d, %Y"}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Display date in `US Style`.

### Output

<img src="../assets/images/options/format_types__date__default--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:format_types__date__default => {:strf => "%m/%d/%Y"}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :format_types__date__default => {:strf => "%m/%d/%Y"}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Display date in `EU Style`.

### Output

<img src="../assets/images/options/format_types__date__default--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:format_types__date__default => {:strf => "%d.%m.%Y"}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :format_types__date__default => {:strf => "%d.%m.%Y"}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

