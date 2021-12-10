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
    {'title' => 'The Great Goblin',
     'author' => 'This is a Demo Document.',
     'subject' => 'Ecommerce Revenue'},
   'encrypt' => 
    {'user_password' => 'pbA0cAQR99TTngmm3XwUmnRx1BCuYaLQVzn6Z0upd7',
     'owner_password' => 'pbA0cAQR99TTngmm3XwUmnRx1BCuYaLQVzn6Z0upd7',
     'permissions' => 
      {'print_document' => true,
       'modify_contents' => false,
       'copy_contents' => false,
       'modify_annotations' => false}}},
 'invoices' => 
  [{'meta' => 
     {'id' => 'R6827748',
      'qr_code' => 'https://abbott.writeinvoice.com/api/R6827748',
      'headline' => 'R6827748 | Darth Maul',
      'group' => '1998-W06'},
    'date' => 
     {'period' => {'from' => 886028400, 'to' => 883868400},
      'invoice' => 885164400,
      'billing' => 886460400},
    'from' => 
     {'address' => 
       {'name' => 'The Great Goblin',
        'phrase' => 'Optimized exuding focus group',
        'street' => '98298 Bashirian Terrace',
        'city' => '44652-3028 Minhmouth',
        'country' => 'Germany'},
      'bank' => 
       {'name' => 'Hayes-Schumm',
        'iban' => 'GB24DCEE28197737994916',
        'bic' => 'BARBGB2LTOO'},
      'contact' => 
       {'phone' => '(374) 682-0732 x00682',
        'mobile' => '(542) 304-4500 x1681',
        'email' => 'samual.doyle@writeinvoice.com',
        'website' => 'abbott.writeinvoice.com'},
      'tax_id' => '655-12-2174'},
    'to' => 
     {'address' => 
       {'name' => 'Darth Maul',
        'street' => '710 Babara Causeway',
        'city' => '24330 New Isaacmouth',
        'country' => 'Hosnian Prime'},
      'tax_id' => '714-29-2795'},
    'items' => 
     {'articles' => 
       [{'id' => '220-81-5664',
         'name' => 'Awesome Paper Hat',
         'pieces' => 3,
         'single' => 56.37,
         'total' => 169.11},
        {'id' => '121-11-0336',
         'name' => 'Awesome Concrete Pants',
         'pieces' => 4,
         'single' => 53.82,
         'total' => 215.28}],
      'sub_total' => 384.39,
      'shipping_fee' => 1.87,
      'total_net' => 386.26,
      'vat' => 73.39,
      'total_gross' => 459.65}}]}


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
      "title": "The Great Goblin",
      "author": "This is a Demo Document.",
      "subject": "Ecommerce Revenue"
    },
    "encrypt": {
      "user_password": "pbA0cAQR99TTngmm3XwUmnRx1BCuYaLQVzn6Z0upd7",
      "owner_password": "pbA0cAQR99TTngmm3XwUmnRx1BCuYaLQVzn6Z0upd7",
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
        "id": "R6827748",
        "qr_code": "https://abbott.writeinvoice.com/api/R6827748",
        "headline": "R6827748 | Darth Maul",
        "group": "1998-W06"
      },
      "date": {
        "period": {
          "from": 886028400,
          "to": 883868400
        },
        "invoice": 885164400,
        "billing": 886460400
      },
      "from": {
        "address": {
          "name": "The Great Goblin",
          "phrase": "Optimized exuding focus group",
          "street": "98298 Bashirian Terrace",
          "city": "44652-3028 Minhmouth",
          "country": "Germany"
        },
        "bank": {
          "name": "Hayes-Schumm",
          "iban": "GB24DCEE28197737994916",
          "bic": "BARBGB2LTOO"
        },
        "contact": {
          "phone": "(374) 682-0732 x00682",
          "mobile": "(542) 304-4500 x1681",
          "email": "samual.doyle@writeinvoice.com",
          "website": "abbott.writeinvoice.com"
        },
        "tax_id": "655-12-2174"
      },
      "to": {
        "address": {
          "name": "Darth Maul",
          "street": "710 Babara Causeway",
          "city": "24330 New Isaacmouth",
          "country": "Hosnian Prime"
        },
        "tax_id": "714-29-2795"
      },
      "items": {
        "articles": [
          {
            "id": "220-81-5664",
            "name": "Awesome Paper Hat",
            "pieces": 3,
            "single": 56.37,
            "total": 169.11
          },
          {
            "id": "121-11-0336",
            "name": "Awesome Concrete Pants",
            "pieces": 4,
            "single": 53.82,
            "total": 215.28
          }
        ],
        "sub_total": 384.39,
        "shipping_fee": 1.87,
        "total_net": 386.26,
        "vat": 73.39,
        "total_gross": 459.65
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