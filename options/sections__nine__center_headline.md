---
sort: 95
title: F.6 sections__nine__center_headline
---
# sections__nine__center_headline

Set Headline of the `center footer column`.


## Preview

<div >
    <canvas id='canvas' search=':sections__nine__center_headline' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__nine__center_headline => 
  {:content => nil,
   :struct => "<b><<--a-->></b>",
   :assigns => [{:value => :obj__text__footer__center, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__nine__center_headline``` |  [Sections](./#sections) | [Footer](/sections/footer) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__center, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Underline `<u>` headline.

### Output

<img src="../assets/images/options/sections__nine__center_headline--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__center_headline =>   {:content => nil,   :struct => "<u><<--a-->></u>",   :assigns => [{:value => :obj__text__footer__center, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__center_headline => 
  {:content => nil,
   :struct => "<u><<--a-->></u>",
   :assigns => [{:value => :obj__text__footer__center, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change pointer to `:obj__text__footer__left`.

### Output

<img src="../assets/images/options/sections__nine__center_headline--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__center_headline =>   {:content => nil,   :struct => "<b><<--a-->></b>",   :assigns => [{:value => :obj__text__footer__left, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__center_headline => 
  {:content => nil,
   :struct => "<b><<--a-->></b>",
   :assigns => [{:value => :obj__text__footer__left, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

