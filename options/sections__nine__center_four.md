---
sort: 99
title: F.10 sections__nine__center_four
---
# sections__nine__center_four

Set the `fourth row` of the center footer column.


## Preview

<div >
    <canvas id='canvas' search=':sections__nine__center_four' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__nine__center_four => 
  {:content => nil,
   :struct => "<b><<--a-->> <<--b-->></b>",
   :assigns => 
    [{:value => :obj__text__tax_id, :format => nil},
     {:value => :payload__from__tax_id, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__nine__center_four``` |  [Sections](./#sections) | [Footer](/sections/footer) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<b><<--a-->> <<--b-->></b>", :assigns=>[{:value=>:obj__text__tax_id, :format=>nil}, {:value=>:payload__from__tax_id, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Underline `<u>` text.

### Output

<img src="../assets/images/options/sections__nine__center_four--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__center_four =>   {:content => nil,   :struct => "<u><<--a-->></u> <<--b-->>",   :assigns =>     [{:value => :obj__text__tax_id, :format => nil},     {:value => :payload__from__tax_id, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__center_four => 
  {:content => nil,
   :struct => "<u><<--a-->></u> <<--b-->>",
   :assigns => 
    [{:value => :obj__text__tax_id, :format => nil},
     {:value => :payload__from__tax_id, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Insert text: `ID`.

### Output

<img src="../assets/images/options/sections__nine__center_four--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__nine__center_four =>   {:content => nil,   :struct => "<u>ID:</u> <<--a-->>",   :assigns => [{:value => :payload__from__tax_id, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__nine__center_four => 
  {:content => nil,
   :struct => "<u>ID:</u> <<--a-->>",
   :assigns => [{:value => :payload__from__tax_id, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

