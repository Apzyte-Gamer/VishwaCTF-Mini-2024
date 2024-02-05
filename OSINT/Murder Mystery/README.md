Murder Mystery
=

The renowned figure in our nation has fallen victim to a heinous crime. An anonymous sender has delivered a letter, hinting at possible knowledge regarding the identity of the KILLER. Your quest is to unravel this Murder Mystery and apprehend the elusive killer.

Author : Aditya Ingale (@adiraj_958)

### FLAG FORMAT: VishwaCTF{Name of the killer}
### Attachements:
#### 1) [letter.txt](letter.txt)
#### 2) [letter.jpg](letter.jpg)

Solution
=

At first, I opened the `letter.jpg` file to find an envelope with a barcode. I scanned the barcode and got this stuff:

```
Barcode ID:    10
Special Services:    111
Mailer ID:    810510
Serial Number:    895115104
Delivery Point ZIP Code:    97100111119
```

This stuff wasn't real, so I went on to reading the `letter.txt` file. It said we had to `decode` the killers name. So, that's when an idea popped me, to concatenate the values after scanning the barcode.

The concatenated numbers were `1011181051089511510497100111119`. By Ascii decoding this, we get the text as `evil_shadow`. By this we get our flag!

`VishwaCTF{evil_shadow}`
