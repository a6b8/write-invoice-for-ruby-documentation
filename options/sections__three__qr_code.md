---
sort: 113
title: F.24 sections__three__qr_code
---
# sections__three__qr_code

Define text for `"QR Code"` in section "three".


## Preview

<div >
    <canvas id='canvas' search=':sections__three__qr_code' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :sections__three__qr_code => 
  {:content => nil,
   :struct => "<<--a-->>",
   :assigns => [{:value => :payload__meta__qr_code, :format => nil}]}
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:sections__three__qr_code``` |  [Sections](./#sections) | [Three](/sections/three) |

### Value



| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```{:content=>nil, :struct=>"<<--a-->>", :assigns=>[{:value=>:payload__meta__qr_code, :format=>nil}]}``` | ```^{a-zA-Z0-9}*$``` | Hash |

## Example A.

Add `#test-123` to url.

### Output

<img src="../assets/images/options/sections__three__qr_code--a.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__three__qr_code =>   {:content => nil,   :struct => "<<--a-->>#test-123",   :assigns => [{:value => :payload__meta__qr_code, :format => nil}]}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__three__qr_code => 
  {:content => nil,
   :struct => "<<--a-->>#test-123",
   :assigns => [{:value => :payload__meta__qr_code, :format => nil}]}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

## Example B.

Insert `VCard`.

### Output

<img src="../assets/images/options/sections__three__qr_code--b.png">



### Parameters

| | **Value** | **Type** |
|------:|:------|:------|
| **Output** | 'my-invoice.pdf' | String |
| **Payload** | {...} [see Payload](../payload) | hash |
| **Options** | ```{:sections__three__qr_code =>   {:content => nil,   :struct =>     "BEGIN:VCARD VERSION:3.0 N:User;Test FN:Test User ORG:13p4 Organisation TITLE:Title [title] REV:20121015T195243Z END:VCARD",   :assigns => []}}``` | hash |


### Source Code

* Invoke Function

```ruby
require 'write_invoice'
 
pyld = WriteInvoice::Example.generate()
opts = {
 :sections__three__qr_code => 
  {:content => nil,
   :struct => 
    "BEGIN:VCARD VERSION:3.0 N:User;Test FN:Test User ORG:13p4 Organisation TITLE:Title [title] REV:20121015T195243Z END:VCARD",
   :assigns => []}
}
 
WriteInvoice::Document.generate( output: 'my-invoice.pdf', payload: pyld, options: opts )

```

