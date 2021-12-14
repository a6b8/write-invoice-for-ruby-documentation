---
sort: 3
title: Payload
---

# Payload

```ruby
require 'pp'
require 'write_invoice'

payload = WriteInvoice::Example.generate( invoices_total: 1..1, articles_total: 1..1, debug: true )
puts payload.pretty_inspect
```

| Name | Type| Default | Required |
| :-- | :-- | :-- | :-- |
| `invoices_total:` | Range | `3..6` | no | 
| `articles_total:` | Range | `2..6` | no |
| `debug:` | Boolean | `true` | no | 


## Preview

<div>
    <canvas id="canvas" search="" palette="payload_overview"></canvas>
</div>
<script src="../assets/js/marker.js"></script>  


## Example
This is a fictional payload which is generated with ```WriteInvoice::Example.generate()```

*As Ruby Hash*

```ruby
require 'write_invoice'

payload = {
'document' => 
  {'metadata' => 
    {'title' => 'Balin',
     'author' => 'This is a Demo Document.',
     'subject' => 'Ecommerce Revenue'},
   'encrypt' => 
    {'user_password' => 'Uxr7jivvJwS7xdvpMh68Bqd5YtaGsWbynuKLwZLSde',
     'owner_password' => 'Uxr7jivvJwS7xdvpMh68Bqd5YtaGsWbynuKLwZLSde',
     'permissions' => 
      {'print_document' => true,
       'modify_contents' => false,
       'copy_contents' => false,
       'modify_annotations' => false}}},
 'invoices' => 
  [{'meta' => 
     {'id' => 'S8363649',
      'qr_code' => 'https://murray.writeinvoice.com/api/S8363649',
      'headline' => 'S8363649 | Rose Tico',
      'group' => '1998-W08'},
    'date' => 
     {'period' => {'from' => 885423600, 'to' => 885423600},
      'invoice' => 886719600,
      'billing' => 888015600},
    'from' => 
     {'address' => 
       {'name' => 'Balin',
        'phrase' => 'Fully-configurable systematic function',
        'street' => '209 Markus Walks',
        'city' => '94799-9873 New Alex',
        'country' => 'United States of America'},
      'bank' => 
       {'name' => 'Hodkiewicz Group',
        'iban' => 'GB75KODQ94217971207196',
        'bic' => 'BKCHGB2UXXX'},
      'contact' => 
       {'phone' => '1-399-288-0072 x89236',
        'mobile' => '1-808-316-7962 x084',
        'email' => 'oma.toy@writeinvoice.com',
        'website' => 'murray.writeinvoice.com'},
      'tax_id' => '109-79-0901'},
    'to' => 
     {'address' => 
       {'name' => 'Rose Tico',
        'street' => '11974 Veum Island',
        'city' => '55098 Port Joeshire',
        'country' => 'Mustafar'},
      'tax_id' => '631-27-8818'},
    'items' => 
     {'articles' => 
       [{'id' => '276-03-9155',
         'name' => 'Aerodynamic Cotton Coat',
         'pieces' => 3,
         'single' => 80.99,
         'total' => 242.97},
        {'id' => '453-63-3074',
         'name' => 'Aerodynamic Leather Shoes',
         'pieces' => 4,
         'single' => 74.6,
         'total' => 298.4}],
      'sub_total' => 541.37,
      'shipping_fee' => 3.39,
      'total_net' => 544.76,
      'vat' => 103.5,
      'total_gross' => 648.26}}]}


WriteInvoice::Document.generate( output: 'test.pdf', payload: payload, options: {} )
```

*As JSON String*

```ruby
require 'json'
require 'write_invoice'

data = <<-EOS
{
  "document": {
    "metadata": {
      "title": "Balin",
      "author": "This is a Demo Document.",
      "subject": "Ecommerce Revenue"
    },
    "encrypt": {
      "user_password": "Uxr7jivvJwS7xdvpMh68Bqd5YtaGsWbynuKLwZLSde",
      "owner_password": "Uxr7jivvJwS7xdvpMh68Bqd5YtaGsWbynuKLwZLSde",
      "permissions": {
        "print_document": true,
        "modify_contents": false,
        "copy_contents": false,
        "modify_annotations": false
      }
    }
  },
  "invoices": [
    {
      "meta": {
        "id": "S8363649",
        "qr_code": "https://murray.writeinvoice.com/api/S8363649",
        "headline": "S8363649 | Rose Tico",
        "group": "1998-W08"
      },
      "date": {
        "period": {
          "from": 885423600,
          "to": 885423600
        },
        "invoice": 886719600,
        "billing": 888015600
      },
      "from": {
        "address": {
          "name": "Balin",
          "phrase": "Fully-configurable systematic function",
          "street": "209 Markus Walks",
          "city": "94799-9873 New Alex",
          "country": "United States of America"
        },
        "bank": {
          "name": "Hodkiewicz Group",
          "iban": "GB75KODQ94217971207196",
          "bic": "BKCHGB2UXXX"
        },
        "contact": {
          "phone": "1-399-288-0072 x89236",
          "mobile": "1-808-316-7962 x084",
          "email": "oma.toy@writeinvoice.com",
          "website": "murray.writeinvoice.com"
        },
        "tax_id": "109-79-0901"
      },
      "to": {
        "address": {
          "name": "Rose Tico",
          "street": "11974 Veum Island",
          "city": "55098 Port Joeshire",
          "country": "Mustafar"
        },
        "tax_id": "631-27-8818"
      },
      "items": {
        "articles": [
          {
            "id": "276-03-9155",
            "name": "Aerodynamic Cotton Coat",
            "pieces": 3,
            "single": 80.99,
            "total": 242.97
          },
          {
            "id": "453-63-3074",
            "name": "Aerodynamic Leather Shoes",
            "pieces": 4,
            "single": 74.6,
            "total": 298.4
          }
        ],
        "sub_total": 541.37,
        "shipping_fee": 3.39,
        "total_net": 544.76,
        "vat": 103.5,
        "total_gross": 648.26
      }
    }
  ]
}
EOS

payload = JSON.parse( data )
WriteInvoice::Document.generate( output: 'test.pdf', payload: payload, options: {} )
```


## Structure

```ruby
    payload = {
        document: {
            metadata: {
                title: '',
                author: '',
                subject: ''
            },
            encrypt: {
                user_password: '',
                owner_password: '',
                permissions: {
                    print_document: boolean,
                    modify_contents: boolean,
                    copy_contents: boolean,
                    modify_annotations: boolean
                }
            }
        },
        invoices: [
            {
                meta: {
                    id: '',
                    qr_code: '',
                    headline: '',
                    group: ''
                },
                date: {
                    period: {
                        from: 0, 
                        to: 0
                    },
                    invoice: 0,
                    billing: 0
                },
                from: {
                    address: {
                        name: '',
                        phrase: '',
                        street: '',
                        city: '',
                        country: ''
                    },
                    bank: {
                        name: '',
                        iban: '',
                        bic: ''
                    },
                    contact: {
                        phone: '',
                        mobile: '',
                        email: '',
                        website: ''
                    },
                    tax_id: ''
                },
                to: {
                    address: {
                        name: '',
                        street: '',
                        city: '',
                        country: ''
                    },
                    tax_id: ''
                },
                items: {
                    articles: [
                        {
                            id: '',
                            name: '',
                            pieces: 0,
                            single: 0.00,
                            total: 0.00
                        },                    
                    ],
                    sub_total: 0.00,
                    shipping_fee: 0.00,
                    total_net: 0.00,
                    vat: 0.00,
                    total_gross: 0.00
                }
            }
        ]
    }
```