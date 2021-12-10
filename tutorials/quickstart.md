---
sort: 1
title: Quickstart
---

# Quickstart


## Overview
Fastest Way to get started:
- Install gem with `gem install write_invoice`
- Generate Payload with `WriteInvoice::Example.generate()`
- Generate Document with `WriteInvoice::Document.generate()`

*Observe all options and payload datapoints here: [sections/](../sections/)*

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


### 3: Generate Document

*To Storage*

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
WriteInvoice::Document.generate( output: 'test.pdf', payload: pyld, options: {} )
```

*To Memory*

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
doc = WriteInvoice::Document.generate( payload: pyld, options: {} )
File.open( 'test.pdf', "w" ) { | f | f.write( doc ) }
```