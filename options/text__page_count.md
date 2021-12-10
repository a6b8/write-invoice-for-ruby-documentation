---
sort: 17
title: C.7 text__page_count
---
# text__page_count

Set Page count output here. Use `<page>` to show current page number and `<total>` to show sum of all pages.


## Preview

<div >
    <canvas id='canvas' search=':text__page_count' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :text__page_count => "<page> / <total>"
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:text__page_count``` |  [Text](./#text) | [Header](/sections/header) |

### Value

Allow A-Z, a-b and 0-9 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```"<page> / <total>"``` | ```^[a-zA-Z0-9_]*$``` | String |

## Example A.

Change Text to `of`.

### Output

<img src="../assets/images/options/text__page_count--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:text__page_count => "<page> of <total> "}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :text__page_count => "<page> of <total> "
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Show only `<page>`.

### Output

<img src="../assets/images/options/text__page_count--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:text__page_count => "Page: <page>"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :text__page_count => "Page: <page>"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

