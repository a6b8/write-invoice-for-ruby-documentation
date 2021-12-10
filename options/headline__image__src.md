---
sort: 127
title: G.9 headline__image__src
---
# headline__image__src

Set local `image path` for company logo, use .png or .jpg


## Preview

<div >
    <canvas id='canvas' search=':headline__image__src' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :headline__image__src => ""
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:headline__image__src``` |  [Headline](./#headline) | [Header](/sections/header) |

### Value

Allow A-Z, a-b and 0-9 as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```""``` | ```^[a-zA-Z0-9_]*$``` | String |

## Example A.

Show Logo

### Output

<img src="../assets/images/options/headline__image__src--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:show__logo => true, :headline__image__src => "<<--ROOT-->__generate/files/templates/logo.png"}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :show__logo => true,
 :headline__image__src => "<<--ROOT-->__generate/files/templates/logo.png"
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

