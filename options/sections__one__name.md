---
sort: 118
title: F.29 sections__one__name
---
# sections__one__name

Define text in section "one" (header)


## Preview

<div >
    <canvas id='canvas' search=':sections__one__name' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__one__name => 
  {:content => nil,
   :struct => "<b><<--a-->></b>\n" + "<<--b-->>\n" + "<<--c-->>\n" + "<<--d-->>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__phrase, :format => nil},
     {:value => :payload__from__address__city, :format => nil},
     {:value => :payload__from__address__country, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__one__name``` |  [Sections](./#sections) | [Header](/sections/header) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<b><<--a-->></b>\n<<--b-->>\n<<--c-->>\n<<--d-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}, {:value=>:payload__from__address__phrase, :format=>nil}, {:value=>:payload__from__address__city, :format=>nil}, {:value=>:payload__from__address__country, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Underline `<u>` text.

### Output

<img src="../assets/images/options/sections__one__name--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__one__name =>   {:content => nil,   :struct => "<u><<--a-->></u>\n" + "<<--b-->>\n" + "<<--c-->>\n" + "<<--d-->>",   :assigns =>     [{:value => :payload__from__address__name, :format => nil},     {:value => :payload__from__address__phrase, :format => nil},     {:value => :payload__from__address__city, :format => nil},     {:value => :payload__from__address__country, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__one__name => 
  {:content => nil,
   :struct => "<u><<--a-->></u>\n" + "<<--b-->>\n" + "<<--c-->>\n" + "<<--d-->>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__phrase, :format => nil},
     {:value => :payload__from__address__city, :format => nil},
     {:value => :payload__from__address__country, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Modify text.

### Output

<img src="../assets/images/options/sections__one__name--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__one__name =>   {:content => nil,   :struct => "<u><<--a-->></u>\n" + "<<--b-->>",   :assigns =>     [{:value => :payload__from__address__name, :format => nil},     {:value => :payload__from__address__phrase, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__one__name => 
  {:content => nil,
   :struct => "<u><<--a-->></u>\n" + "<<--b-->>",
   :assigns => 
    [{:value => :payload__from__address__name, :format => nil},
     {:value => :payload__from__address__phrase, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

