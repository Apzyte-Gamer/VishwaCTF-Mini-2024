Looking for Dushyanta
=

I was always fascinated by how a certain Indian artist combined Eurpoean realism with Indian sensibility. But this fascination wasn't enough help me remember the artist's name. Maybe you could give me a tip to score good in art histroy exams.

Author : Amruta Patil (@renegade.0_0)

### FLAG FORMAT: VishwaCTF{}
### Attachement: [looking_for_Dushyanta.jpg](https://vishwactf.s3.amazonaws.com/files/attachments/looking_for_Dushyanta_5ec6c684-c947-4200-b6d2-9ad7643d02f6.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T191813Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=9fa56c61398d65aa4ab202ae4678ebbbbbe6ccbc93699284489d9908d105b2e6)

Solution
=

The image is an art piece drawn by Ravi Sharma in 1898. It is nothing on its own, until we run stegseek to find any usefull info on it and we find this supposed Keyed Cipher. `sy+15+_d135_lo+_4e+_e1v35_0y`.

Since it is a Keyed Cipher, we need a key for it, and luckily its `SHAKUNTALA` since she is the one in the photo.

By using many ciphers, there was nothing, until Vignere worked! I put on the cipher and the key and got the flag!

`VishwaCTF{ar+15+_d135_bu+_4r+_l1v35_0n}`
