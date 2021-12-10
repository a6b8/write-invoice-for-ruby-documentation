---
sort: 115
title: F.26 sections__three__headline
---
# sections__three__headline

Define `headlinev in section "three".


## Preview

<div >
    <canvas id='canvas' search=':sections__three__headline' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__three__headline => 
  {:content => nil,
   :struct => "<b><<--a-->> | <<--b-->></b>",
   :assigns => 
    [{:value => :obj__text__invoice, :format => nil},
     {:value => :payload__meta__id, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__three__headline``` |  [Sections](./#sections) | [Three](/sections/three) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<b><<--a-->> | <<--b-->></b>", :assigns=>[{:value=>:obj__text__invoice, :format=>nil}, {:value=>:payload__meta__id, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Change text to: `ID:`.

### Output

<img src="../assets/images/options/sections__three__headline--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__three__headline =>   {:content => nil,   :struct => "<b><<--a-->>, ID: <<--b-->></b>",   :assigns =>     [{:value => :obj__text__invoice, :format => nil},     {:value => :payload__meta__id, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__three__headline => 
  {:content => nil,
   :struct => "<b><<--a-->>, ID: <<--b-->></b>",
   :assigns => 
    [{:value => :obj__text__invoice, :format => nil},
     {:value => :payload__meta__id, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Underline `<u>` text.

### Output

<img src="../assets/images/options/sections__three__headline--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__three__headline =>   {:content => nil,   :struct => "<u><<--a-->></u> | ID: <<--b-->>",   :assigns =>     [{:value => :obj__text__invoice, :format => nil},     {:value => :payload__meta__id, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__three__headline => 
  {:content => nil,
   :struct => "<u><<--a-->></u> | ID: <<--b-->>",
   :assigns => 
    [{:value => :obj__text__invoice, :format => nil},
     {:value => :payload__meta__id, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

