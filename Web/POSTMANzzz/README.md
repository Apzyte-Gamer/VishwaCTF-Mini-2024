POSTMANzzz
=

A postman has been assigned a task, and the only details provided are

He has to find the message inside Twitter
He has to post the message. Help him complete his task, and you will be rewarded ...
Author : Saksham Saipatwar (@sss1011)

### FLAG FORMAT: VishwaCTF{}
### Website Instance: https://ch230136857.ch.eng.run/

Solution
=

I at first create a plan of what to do:
1) Find the body
2) POST the body in order to get the flag

Loading up the website, we see an empty home page except from the social media links which lead us to Cybercell VIIT's socials. My first instinct is to check the source code to see any information related to the body that the postman has to post. I scroll down until I find something interesting in the twitter link. 

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/b653b0ce-7723-4f6c-a798-cafc9085d1f4)

I guessed it would be the body so I copied it. I then opened postman and sent a query to the website with the body but nothing. It gave me this message tho: `retry using proper message ... remember to send the message inside body in url-encoded form only !!`. This tells us that its not `body` its `message`. I then go to the `body` section and in the `x-www-form-urlencoded` type, I send the message and get this response: `Message recived sucessfully ... visit /welcome-updated-with-flag to recive your reward`.

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/dfcac60d-0558-47d1-b71f-41758f7da108)

I then went to `https://ch230136857.ch.eng.run/welcome-updated-with-flag` (not in postman but in google) and find nothing. I look at the source code (css file since I hadn't checked it earlier) and find there are 2 backgrounds.

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/d639e3e3-4ee1-4fcf-a8cc-2c0ea2864833)

I then removed the last background and got the flag!

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/474b62a9-0510-42b2-8bbb-246952c21e3c)

`VishwaCTF{POSTM3N_R3MA1N_VA1UAB13_TODAY}`
