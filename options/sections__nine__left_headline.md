---
sort: 90
title: F.1 sections__nine__left_headline
---
# sections__nine__left_headline

Set Headline of the `left footer` column.


## Preview

<div >
    <canvas id='canvas' search=':sections__nine__left_headline' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__nine__left_headline => 
  {:content => nil,
   :struct => "<b><<--a-->></b>",
   :assigns => [{:value => :obj__text__footer__left, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__nine__left_headline``` |  [Sections](./#sections) | [Footer](/sections/footer) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<b><<--a-->></b>", :assigns=>[{:value=>:obj__text__footer__left, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Underline `<u>` headline.

### Output

<img src="../assets/images/options/sections__nine__left_headline--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__left_headline =>   {:content => nil,   :struct => "<u><<--a-->></u>",   :assigns => [{:value => :obj__text__footer__left, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__left_headline => 
  {:content => nil,
   :struct => "<u><<--a-->></u>",
   :assigns => [{:value => :obj__text__footer__left, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Change pointer to `:obj__text__footer__center`.

### Output

<img src="../assets/images/options/sections__nine__left_headline--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__left_headline =>   {:content => nil,   :struct => "<b><<--a-->></b>",   :assigns => [{:value => :obj__text__footer__center, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__left_headline => 
  {:content => nil,
   :struct => "<b><<--a-->></b>",
   :assigns => [{:value => :obj__text__footer__center, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

