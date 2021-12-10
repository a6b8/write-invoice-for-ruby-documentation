---
sort: 5
title: Change your document QR Code text
---

# Change your document QR Code text


## Overview
Quickest way to change your QR Code URL on your doocument is:
- Install gem with `gem install write_invoice`
- Generate Payload with `WriteInvoice::Example.generate()`
- Modify your payload `[:invoices][ 0 ][:meta][:qr_code]`.
- Generate Document with `WriteInvoice::Document.generate()`

*To Hide your QR Code set `show__qr_code: false` visit: [show__qr_code](../options/show__qr_code.html)*


## Steps

### 1: Install gem
Install module from rubygems.

```bash
gem install write_invoice
```


### 2: Generate Payload
Generate a payload with `::example` Class.

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
```


### 3: Payload: Modify QR Code Text

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
pyld[:invoices][ 0 ][:meta][:qr_code] = 'https://docs.writeinvoice.com/options/show__qr_code'

```

### 4: Generate Document

*To Storage*

```ruby
require 'write_invoice'

pyld = WriteInvoie::Example.generate()
pyld[:invoices][ 0 ][:meta][:qr_code] = 'https://docs.writeinvoice.com/options/show__qr_code'

WriteInvoice::Document.generate( output: 'test.pdf', payload: pyld )
```

*To Memory*

```ruby
require 'write_invoice'

pyld = WriteInvoie::Example.generate()
pyld[:invoices][ 0 ][:meta][:qr_code] = 'https://docs.writeinvoice.com/options/show__qr_code'

doc = WriteInvoice::Document.generate( payload: pyld )
File.open( 'test.pdf', "w" ) { | f | f.write( doc ) }
```