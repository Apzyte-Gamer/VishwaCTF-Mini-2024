Murder Mystery
=

The renowned figure in our nation has fallen victim to a heinous crime. An anonymous sender has delivered a letter, hinting at possible knowledge regarding the identity of the KILLER. Your quest is to unravel this Murder Mystery and apprehend the elusive killer.

Author : Aditya Ingale (@adiraj_958)

### FLAG FORMAT: VishwaCTF{Name of the killer}
### Attachements:
#### 1) [letter.txt](https://vishwactf.s3.amazonaws.com/files/attachments/letter_0a363cba-3849-45c8-8b34-1de18adeb1c9.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T185621Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=bc7373ceb177a4129bb8aa37e8424c9ee7966f6599a991533e19bef9e19afd3c)
#### 2) [letter.jpg](https://vishwactf.s3.amazonaws.com/files/attachments/letter_b247ef5e-99f9-4275-8397-c6923eacdc72.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T185721Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=411afbd469e49104f38d64b58d414aa62c950ae262f0a7104adad676c633aae8)

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
