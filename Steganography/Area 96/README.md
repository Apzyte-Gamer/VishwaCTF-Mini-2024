Area 96
=

A confirmed UFO sighting has unveiled the presence of extraterrestrial beings who have transmitted an audio file (AlienMessage.wav) that has stumped government analysts. According to intelligence reports, these aliens are avid music enthusiasts and witty pranksters. Your mission is to decipher the encrypted hidden message they have conveyed to Earth.

NOTE: The passwords are written in ALL CAPS without any spacing

Author: Pranit Govande (@razor_1225)

### FLAG FORMAT: VishwaCTF{}
### Attachements:
1) [AlienMessage.wav](AlienMessage.wav)
2) [flag.jpg](flag.jpg)
3) [Video1.7z](Video1.7z)
4) [Audio2.7z](Audio2.7z)

Solution
=

At first, I tried to extract the .7z's files but they required a password. My teammate then looked at `AlienMessage.wav` to maybe get the password for one of them. He checked the spectogram for it and there was a link embedded there (https://bit.ly/3vaALn5). This link rickrolles us but my teammate has other plans. He guessed password as `RICKASTLEY` and somehow he got the password for `Video1.7z`!

The archive has a parkour video. I then thought that there could be the flag in the flag.jpg as it was named so. So, I went onto `parkour.mp4` thinking I could probably get a hint from there. I used a tool and got a .txt file containing `VIITPUNE`.

I then immediately went onto `flag.jpg` to get any useful info from steghide, but it wasn't the correct pass. So, I instead used it as the pass for `Audio2.7z` and it actually worked and gave me `audiopw.mp3`!

I then opened up `audiopw.mp3` and got a song. I searched the song up on google, and the name of the song was `Praise`. Thinking this was the password for `flag.jpg`, I formatted it to `PRAISE` and gave it a shot.

`VishwaCTF{BeepBoop_Jaadu}`
