Area 96
=

A confirmed UFO sighting has unveiled the presence of extraterrestrial beings who have transmitted an audio file (AlienMessage.wav) that has stumped government analysts. According to intelligence reports, these aliens are avid music enthusiasts and witty pranksters. Your mission is to decipher the encrypted hidden message they have conveyed to Earth.

NOTE: The passwords are written in ALL CAPS without any spacing

Author: Pranit Govande (@razor_1225)

### FLAG FORMAT: VishwaCTF{}
### Attachements:
1) [AlienMessage.wav](https://vishwactf.s3.amazonaws.com/files/attachments/AlienMessage_d25a62af-c03e-4956-a5d7-1fa431f2ec61.wav?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T192707Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=52edde92c2dd0b99d55099bd96c0f55848cd998008c39401d22507bf83803c8a)
2) [flag.jpg](https://vishwactf.s3.amazonaws.com/files/attachments/flag_4742952d-2a1e-4147-8b1a-2ccc0f72ac8e.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T192723Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=152c6f3f0d0b3fb53dbcc1f3b9be57695e5eb36854f4adf2c43577d6baba833f)
3) [Video1.7z](https://vishwactf.s3.amazonaws.com/files/attachments/Video1_5afd8363-ede4-443c-9863-3d79695af4b0.7z?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T192738Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=e29db9c93210661b35b0008ad4787d6f6def1fcaa9c7d2f4814b379c56c26723)
4) [Audio2.7z](https://vishwactf.s3.amazonaws.com/files/attachments/Audio2_7856cb2f-5a73-458a-a6b6-47f0651905fb.7z?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA6GUFVMV6HO3NYL6Z%2F20240204%2Fap-south-1%2Fs3%2Faws4_request&X-Amz-Date=20240204T192753Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=6ca6546a801a0bf98d45910e13f7dae2367f1d9c4fa68112c74d249b02768a48)

Solution
=

At first, I tried to extract the .7z's files but they required a password. My teammate then looked at `AlienMessage.wav` to maybe get the password for one of them. He checked the spectogram for it and there was a link embedded there (https://bit.ly/3vaALn5). This link rickrolles us but my teammate has other plans. He guessed password as `RICKASTLEY` and somehow he got the password for `Video1.7z`!

The archive has a parkour video. I then thought that there could be the flag in the flag.jpg as it was named so. So, I went onto `parkour.mp4` thinking I could probably get a hint from there. I used a tool and got a .txt file containing `VIITPUNE`.

I then immediately went to `flag.jpg`, and used steghide to get the flag!

`VishwaCTF{BeepBoop_Jaadu}`
