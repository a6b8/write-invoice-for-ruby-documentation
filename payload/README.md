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
    {'title' => 'Gloin',
     'author' => 'This is a Demo Document.',
     'subject' => 'Ecommerce Revenue'},
   'encrypt' => 
    {'user_password' => 'yoUGvrd4mCdmDpsKdQCb8IpmccoOMELyXZaDOzG7Pn',
     'owner_password' => 'yoUGvrd4mCdmDpsKdQCb8IpmccoOMELyXZaDOzG7Pn',
     'permissions' => 
      {'print_document' => true,
       'modify_contents' => false,
       'copy_contents' => false,
       'modify_annotations' => false}}},
 'invoices' => 
  [{'meta' => 
     {'id' => 'Z8012530',
      'qr_code' => 'https://gerhold.writeinvoice.com/api/Z8012530',
      'headline' => 'Z8012530 | Shmi Skywalker',
      'group' => '1998-W05'},
    'date' => 
     {'period' => {'from' => 885942000, 'to' => 883609200},
      'invoice' => 884905200,
      'billing' => 886201200},
    'from' => 
     {'address' => 
       {'name' => 'Gloin',
        'phrase' => 'Organized scalable solution',
        'street' => '427 Nohemi Roads',
        'city' => '24143-8384 Port Enriquetaville',
        'country' => 'Bahrain'},
      'bank' => 
       {'name' => 'Walsh Inc',
        'iban' => 'GB28JGIY54534983728417',
        'bic' => 'AAQIGB21'},
      'contact' => 
       {'phone' => '1-150-026-4587 x55676',
        'mobile' => '1-590-444-4750 x42378',
        'email' => 'damien.haley@writeinvoice.com',
        'website' => 'gerhold.writeinvoice.com'},
      'tax_id' => '457-66-6720'},
    'to' => 
     {'address' => 
       {'name' => 'Shmi Skywalker',
        'street' => '3574 Harvey Forest',
        'city' => '15556-9831 Terriberg',
        'country' => 'Ahch-To'},
      'tax_id' => '707-45-6564'},
    'items' => 
     {'articles' => 
       [{'id' => '050-20-0832',
         'name' => 'Sleek Leather Pants',
         'pieces' => 5,
         'single' => 31.14,
         'total' => 155.7},
        {'id' => '366-47-1813',
         'name' => 'Small Granite Bottle',
         'pieces' => 5,
         'single' => 30.14,
         'total' => 150.7}],
      'sub_total' => 306.4,
      'shipping_fee' => 2.45,
      'total_net' => 308.85,
      'vat' => 58.68,
      'total_gross' => 367.53}}]}


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
      "title": "Gloin",
      "author": "This is a Demo Document.",
      "subject": "Ecommerce Revenue"
    },
    "encrypt": {
      "user_password": "yoUGvrd4mCdmDpsKdQCb8IpmccoOMELyXZaDOzG7Pn",
      "owner_password": "yoUGvrd4mCdmDpsKdQCb8IpmccoOMELyXZaDOzG7Pn",
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
        "id": "Z8012530",
        "qr_code": "https://gerhold.writeinvoice.com/api/Z8012530",
        "headline": "Z8012530 | Shmi Skywalker",
        "group": "1998-W05"
      },
      "date": {
        "period": {
          "from": 885942000,
          "to": 883609200
        },
        "invoice": 884905200,
        "billing": 886201200
      },
      "from": {
        "address": {
          "name": "Gloin",
          "phrase": "Organized scalable solution",
          "street": "427 Nohemi Roads",
          "city": "24143-8384 Port Enriquetaville",
          "country": "Bahrain"
        },
        "bank": {
          "name": "Walsh Inc",
          "iban": "GB28JGIY54534983728417",
          "bic": "AAQIGB21"
        },
        "contact": {
          "phone": "1-150-026-4587 x55676",
          "mobile": "1-590-444-4750 x42378",
          "email": "damien.haley@writeinvoice.com",
          "website": "gerhold.writeinvoice.com"
        },
        "tax_id": "457-66-6720"
      },
      "to": {
        "address": {
          "name": "Shmi Skywalker",
          "street": "3574 Harvey Forest",
          "city": "15556-9831 Terriberg",
          "country": "Ahch-To"
        },
        "tax_id": "707-45-6564"
      },
      "items": {
        "articles": [
          {
            "id": "050-20-0832",
            "name": "Sleek Leather Pants",
            "pieces": 5,
            "single": 31.14,
            "total": 155.7
          },
          {
            "id": "366-47-1813",
            "name": "Small Granite Bottle",
            "pieces": 5,
            "single": 30.14,
            "total": 150.7
          }
        ],
        "sub_total": 306.4,
        "shipping_fee": 2.45,
        "total_net": 308.85,
        "vat": 58.68,
        "total_gross": 367.53
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