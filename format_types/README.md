---
sort: 5
title: Format Types
---

# Format Types

**Currency**
```ruby
    insert = {
        delimiter: ".",
        separator: ",",
        precision: 2,
        unit: '',
        format: "%n €"
    }

    options = { formatters__currency__custom: insert }

```
All Formatters under ```:currency``` will be formatted in usage of ```ActiveSupport::NumberHelper.number_to_currency```. You can find more Informations here: https://api.rubyonrails.org/classes/ActiveSupport/NumberHelper.html
<br>
<br>
**Date**

```ruby
    insert = { strf: '%d.%m.%Y' }
    options = { formatters__date__custom: insert }
```

All Formatters under :date will be formatted in usage of ```DateTime.strftime()```. You can find more Informations here: https://apidock.com/ruby/DateTime/strftime

<br>

<a href="#table-of-contents">
<img src="https://raw.githubusercontent.com/a6b8/a6b8/main/docs/write-invoice-for-ruby/readme/headlines/string-modification.svg" height="38px" name="string-modification" alt="String Modification">
</a>
<br>
To place and format variables in a string you can use modifiers.
<br>
<br>
Here an Example how you can transform strings:

```ruby
    euro = 100.00
    date = 1625933028

    struct = "{{a}} is not much money in {{b}}!"

    # => "100 € is not much in 2021"``
```

### Set new modifier

To create a modifier you need a ```struct``` string and ```assigns``` which articulate the variable input and format. If you dont need a format set the value of ```format: nil```. As placeholder use chars in alphabetic order.

```ruby
    insert = {
        content: nil,
        struct: "{{a}} is not much <u>money</u> in {{b}}!",
        assigns: [
            {
                value: :payload__items__subtotal,
                format: :obj__formatters__currency__short
            },
            {
                value: :payload__meta__date,
                format: :obj__formatters__date__year
            }
        ]
    }

    options = { 
        sections__four__snippet: insert 
    }
```
<br>