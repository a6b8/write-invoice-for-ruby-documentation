---
sort: 116
title: F.27 sections__two__small
---
# sections__two__small

Define address label (from) in section "two"


## Preview

<div >
    <canvas id='canvas' search=':sections__two__small' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__two__small => 
  {:content => nil,
   :struct => "<u><<--a-->> - <<--b-->> - <<--c-->></u>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__street, :format => nil},
     {:value => :payload__from__address__city, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__two__small``` |  [Sections](./#sections) | [Two](/sections/two) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<u><<--a-->> - <<--b-->> - <<--c-->></u>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__from__address__street, :format=>nil}, {:value=>:payload__from__address__city, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Modify text to `bold <b>`.

### Output

<img src="../assets/images/options/sections__two__small--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__two__small =>   {:content => nil,   :struct => "<b><<--a-->> - <<--b-->> - <<--c-->></b>",   :assigns =>     [{:value => :payload__from__address__name, :format => nil},     {:value => :payload__from__address__street, :format => nil},     {:value => :payload__from__address__city, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__two__small => 
  {:content => nil,
   :struct => "<b><<--a-->> - <<--b-->> - <<--c-->></b>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__street, :format => nil},
     {:value => :payload__from__address__city, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Insert Text: `Sender`.

### Output

<img src="../assets/images/options/sections__two__small--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__two__small =>   {:content => nil,   :struct => "Sender: <<--a-->> - <<--b-->> - <<--c-->>",   :assigns =>     [{:value => :payload__from__address__name, :format => nil},     {:value => :payload__from__address__street, :format => nil},     {:value => :payload__from__address__city, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__two__small => 
  {:content => nil,
   :struct => "Sender: <<--a-->> - <<--b-->> - <<--c-->>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__street, :format => nil},
     {:value => :payload__from__address__city, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

