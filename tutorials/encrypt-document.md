---
sort: 4
title: Encrypt your document
---

# Encrypt your document

## Overview

To enable encryption you need to set 2 parameters:
- Set Passwort in Payload: `payload[:document][:encrypt]`. We use `::Example.generate()` for fast exploring.

```ruby
payload = {
    document: {
        metadata: { ... }
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
    }
    invoices: [ ... ]
}
```

- Enable Encryption in Options: `{ show__unencrypted: false }`



## Steps

### 1: Install gem
Install module from rubygems.

```bash
gem install write_invoice
```


### 2: Generate Example Payload
Generate a payload with `::example` Class.

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
```


### 3: Options: Enable Encryption
Set options as a variable a insert `show__unencrypted: false`

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
opts = { show__unencrypted: false }

```


### 4: Generate Document
Generate `.pdf` Document with encryption.

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate( invoices_total: 10..12, articles_total: 5..10 )
opts = { show__unencrypted: false }

WriteInvoice::Document.generate( output: 'test.pdf', payload: pyld, options: opts )
```