Looking for Dushyanta
=

I was always fascinated by how a certain Indian artist combined Eurpoean realism with Indian sensibility. But this fascination wasn't enough help me remember the artist's name. Maybe you could give me a tip to score good in art histroy exams.

Author : Amruta Patil (@renegade.0_0)

### FLAG FORMAT: VishwaCTF{}
### Attachement: [looking_for_Dushyanta.jpg](looking_for_Dushyanta.jpg)

Solution
=

The image is an art piece drawn by Ravi Sharma in 1898. It is nothing on its own, until we run stegseek to find any usefull info on it and we find this supposed Keyed Cipher. `sy+15+_d135_lo+_4e+_e1v35_0y`.

Since it is a Keyed Cipher, we need a key for it, and luckily its `SHAKUNTALA` since she is the one in the photo.

By using many ciphers, there was nothing, until Vignere worked! I put on the cipher and the key and got the flag!

`VishwaCTF{ar+15+_d135_bu+_4r+_l1v35_0n}`
