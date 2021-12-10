<img src="./assets/images/logo.png" height="60px">


`write_invoice` is a ruby gem to generate multiple invoices in one document.
 
:heavy_check_mark: Highly customizable

:heavy_check_mark: More then [200(!) Examples](../options/#categories) available.

:heavy_check_mark: Unique QR Code on every invoice.

:heavy_check_mark: Encrypt your Document

:heavy_check_mark: Watermark function for test purposes.


## Source Code

```bash
gem install write_invoice
```

```ruby
require 'write_invoice'

pyld = WriteInvoice::Example.generate()
doc = WriteInvoice::Document.generate( payload: pyld )
File.open( 'test.pdf', 'w' ) { | f | f.write( doc ) }
```


## Links

[Github](https://github.com/a6b8/write-invoice-for-ruby) <br>
[RubyGems](https://rubygems.org/gems/write_invoice)