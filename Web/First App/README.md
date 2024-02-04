First App
=

After struggling for 2 days finally made my first web page. Still wondering why did I use Linux to host this.

Author : Ankush Kaudi (@itsbunny07)

### FLAG FORMAT: VishwaCTF{}
### Website Instance: https://ch170136859.ch.eng.run/

Solution
=

Opening up the website, I was greeted by a marquee and an input box. I put `test` in it and got `Hi, test I believe you are enjoying our CTF. Wish you all the best for further challenges :)`. My first instinct was to maybe inject SQLi to get the flag maybe, but soon figured it didn't work.

Looking at the description again, I saw it said `Still wondering why did I use *Linux* to host this.`. This gave me an idea that the app has a command injection vulnerability. Looking at the source code, I can see the app gives a request to read the `fl4gf0rF1r5t4pp.php` file. 

I first tried `cat fl4gf0rF1r5t4pp.php`, but it gave me a failure message `Impressive.... Most common way to read files but this will not work here. Maybe you find some other alternatives.`. I then looked for other alternatives until my teammate found out that the command is `batcat`, another popular way to copy contents of a file in linux. By checking, it can be seen that `batcat fl4gf0rF1r5t4pp.php` works and gives us the flag!

`VishwaCTF{1_just_re4lis3d_1_f*ck3d_up_my_4pplic4t10n}`
