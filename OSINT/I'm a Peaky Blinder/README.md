![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/fc54c1f3-4c02-432c-9f2b-78f718c64752)I'm a Peaky Blinder
=

Take a little walk to the edge of town
Go across the tracks
Where the viaduct looms,
like a 00_bird_of_doom_
As it shifts and cracks
Where secrets lie in the border fires,
in the humming wires
Hey man, you know
you're never coming back
Past the square, past the bridge,
past the mills, past the stacks
On a gathering storm comes
a tall handsome man
In a dusty black coat with
a _red_right_hand_00

Replace use _ instead of space

Author : Abhinav (@.0_0.ace.0_0. )

### FLAG FORMAT: VishwaCTF{}

Solution
=

As always, I looked for interesting things in the description and found particularly 2. `_red_right_hand_00` and `00_bird_of_doom_`. As a natural instinct and past experiences, I searched these accounts on instagram, until I found one account named [`_red_right_hand_00`](https://www.instagram.com/_red_right_hand_00/). 

By looking at its posts, we find that there's a part of an URL in every post. By concatenating them, we get a facebook page. https://www.facebook.com/profile.php?id=61554610571803&mibextid=hIlR13.

By looking at Paul Anderson's posts, we can see that there is an instagram link linking to another account. https://www.instagram.com/_t_m_s_00?igsh=MWtncGh4aHhrNmtv

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/92ef84fa-f698-4787-90fc-c587216bdcbb)

We can then see a post in `_t_m_s_00`'s profile containing a question.

![image](https://github.com/Apzyte-Gamer/VishwaCTF-Mini-2024/assets/71684682/bc0c923c-4b5f-4b2f-a2c6-40e2966a1c9f)

The answer to it is the `The Garrison`. Hence, by putting it as the flag, we got our answer!

`VishwaCTF{The_Garrison}`

