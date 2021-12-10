---
sort: 9
title: A.9 show__unencrypted
---
# show__unencrypted

Encrypt or unencrypt .pdf document. To set a password visit [Payload](../payload/#example) #example > document > encrypted


## Preview

<div >
    <canvas id='canvas' search=':show__unencrypted' palette='option_detail'></canvas>
</div>
<script src="../assets/js/marker.js"></script>  

 
## Default

### Hash

```ruby
{
 :show__unencrypted => true
} 
```

### Key

| **Name** | **Category** | **Section** |
| :--- | :--- | :--- |
| ```:show__unencrypted``` |  [Show](./#show) | [Header](/sections/header) |

### Value

Allow true or false as value.

| **Default**| **Validation**| **Type** |
| :--- | :--- | :--- |
| ```true``` | ```^(?:true|false)``` | Boolean |

