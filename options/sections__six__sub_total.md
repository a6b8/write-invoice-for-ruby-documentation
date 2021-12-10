---
sort: 107
title: F.18 sections__six__sub_total
---
# sections__six__sub_total

Define text for area `"Sub Total"` in section "six".


## Preview

<div >
    <canvas id='canvas' search=':sections__six__sub_total' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__six__sub_total => 
  {:content => nil,
   :struct => "<<--a-->>",
   :assigns => 
    [{:value => :payload__items__sub_total,
      :format => :obj__format_types__currency__short}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__six__sub_total``` |  [Sections](./#sections) | [Six](/sections/six) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__items__sub_total, :format=>:obj__format_types__currency__short}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Underline `<u>` text.

### Output

<img src="../assets/images/options/sections__six__sub_total--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__six__sub_total =>   {:content => nil,   :struct => "<u><<--a-->></u>",   :assigns =>     [{:value => :payload__items__sub_total,      :format => :obj__format_types__currency__short}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__six__sub_total => 
  {:content => nil,
   :struct => "<u><<--a-->></u>",
   :assigns => 
    [{:value => :payload__items__sub_total,
      :format => :obj__format_types__currency__short}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Insert text: `Test:`.

### Output

<img src="../assets/images/options/sections__six__sub_total--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__six__sub_total =>   {:content => nil,   :struct => "<b>Test:</b> <<--a-->>",   :assigns =>     [{:value => :payload__items__sub_total,      :format => :obj__format_types__currency__short}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__six__sub_total => 
  {:content => nil,
   :struct => "<b>Test:</b> <<--a-->>",
   :assigns => 
    [{:value => :payload__items__sub_total,
      :format => :obj__format_types__currency__short}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

