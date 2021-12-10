---
sort: 105
title: F.16 sections__eight__snippet
---
# sections__eight__snippet

Define text for section eight.


## Preview

<div >
    <canvas id='canvas' search=':sections__eight__snippet' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__eight__snippet => 
  {:content => nil,
   :struct => 
    "Thank you for using <<--a-->> Services.\n" +
    "\n" +
    "\n" +
    "Sincerely,\n" +
    "\n" +
    "<<--a-->>",
   :assigns => [{:value => :payload__from__address__name, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__eight__snippet``` |  [Sections](./#sections) | [Eight](/sections/eight) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"Thank you for using <<--a-->> Services.\n\n\nSincerely,\n\n<<--a-->>", :assigns=>[{:value=>:payload__from__address__name, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Make text `bold <b>`.

### Output

<img src="../assets/images/options/sections__eight__snippet--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__eight__snippet =>   {:content => nil,   :struct =>     "Thank you for <b>not</b> using <<--a-->> Services.\n" +    "\n" +    "\n" +    "Sincerely,\n" +    "\n" +    "<<--a-->>",   :assigns => [{:value => :payload__from__address__name, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__eight__snippet => 
  {:content => nil,
   :struct => 
    "Thank you for <b>not</b> using <<--a-->> Services.\n" +
    "\n" +
    "\n" +
    "Sincerely,\n" +
    "\n" +
    "<<--a-->>",
   :assigns => [{:value => :payload__from__address__name, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Underline `<u>` text.

### Output

<img src="../assets/images/options/sections__eight__snippet--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__eight__snippet =>   {:content => nil,   :struct =>     "Thank you for using <u><<--a-->> Services</u>.\n" +    "\n" +    "\n" +    "Sincerely,\n" +    "\n" +    "<<--a-->>",   :assigns => [{:value => :payload__from__address__name, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__eight__snippet => 
  {:content => nil,
   :struct => 
    "Thank you for using <u><<--a-->> Services</u>.\n" +
    "\n" +
    "\n" +
    "Sincerely,\n" +
    "\n" +
    "<<--a-->>",
   :assigns => [{:value => :payload__from__address__name, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

