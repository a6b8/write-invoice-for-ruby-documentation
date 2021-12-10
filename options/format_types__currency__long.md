---
sort: 84
title: E.2 format_types__currency__long
---
# format_types__currency__long

Define Format Type for viewing currency values in a `long form`.


## Preview

<div >
    <canvas id='canvas' search=':format_types__currency__long' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :format_types__currency__long => 
  {:delimiter => ".",
   :separator => ",",
   :precision => 2,
   :unit => "",
   :format => "%n EUR"}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:format_types__currency__long``` |  [Format Types](./#format_types) | [Seven](/sections/seven) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:delimiter=>".", :separator=>",", :precision=>2, :unit=>"", :format=>"%n EUR"}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Change currency to `"USD"`.

### Output

<img src="../assets/images/options/format_types__currency__long--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:format_types__currency__long =>   {:delimiter => ".",   :separator => ",",   :precision => 2,   :unit => "",   :format => "%n USD"}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :format_types__currency__long => 
  {:delimiter => ".",
   :separator => ",",
   :precision => 2,
   :unit => "",
   :format => "%n USD"}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change currency to `"YEN"`.

### Output

<img src="../assets/images/options/format_types__currency__long--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:format_types__currency__long =>   {:delimiter => ".",   :separator => ",",   :precision => 2,   :unit => "",   :format => "%n YEN"}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :format_types__currency__long => 
  {:delimiter => ".",
   :separator => ",",
   :precision => 2,
   :unit => "",
   :format => "%n YEN"}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

