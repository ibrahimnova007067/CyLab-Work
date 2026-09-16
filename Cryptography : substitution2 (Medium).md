In this space, I will be narrating my full experience with the substitution2 challenge.
So, since this is a learning path of its own (Substitution Series), I'm already familiar with a tool such as a frequency analysis tool.

Alright, here's our challenge :

<img width="1439" height="319" alt="image" src="https://github.com/user-attachments/assets/bc6aecc9-ab80-43bc-b851-4337edd2b522" />

Let's take a look at our file first! 

<img width="1902" height="100" alt="image" src="https://github.com/user-attachments/assets/4bbdadad-554d-4ca9-a46b-ea7e636e1540" />

Oh boy, this is gonna take a while, but I have a pretty handy trick (you'll see).
So, this is our handy tool here!

<img width="1903" height="964" alt="image" src="https://github.com/user-attachments/assets/451ada7a-e06a-4540-8e3d-7106ac3e0d92" />

(Man, the internet is such a blessing)
Let's paste our text here and start analyzing!

<img width="1731" height="878" alt="image" src="https://github.com/user-attachments/assets/dbadfc93-93fe-40a3-b158-14dc42b9ba37" />

Now, my trick. Don't you spot something odd about this set of letters and numbers here? 

<img width="534" height="29" alt="image" src="https://github.com/user-attachments/assets/70474288-bf0e-4738-addd-7bb7b0a8e3af" />

I've realized something. It has curly brackets, underscores, non-substituted numbers and 7 letters before the brackets. To me, there's no doubt about it - this is our flag!
And since we know flags always start with picoCTF, we've received the answer to 6 letters off the bat!

q = p
t = i
l = c
v = o
l = c
k = t
o = f

<img width="1753" height="321" alt="image" src="https://github.com/user-attachments/assets/acc622e9-8088-47c1-9a29-d86d46c6282d" />

Alright! Now, another thing that stands out to me is this :

<img width="129" height="30" alt="image" src="https://github.com/user-attachments/assets/245efe93-d2f0-4cb0-802e-4ac028400e50" />

There's no way that word isn't competition.

So now, we have :

r = m
j = e
u = n

And now there's another oddball yet again!

<img width="1756" height="307" alt="image" src="https://github.com/user-attachments/assets/fc7fd6d4-3df2-40af-9fb7-73b88cf6a87f" />

That word is practice, right?

e = r
g = a

<img width="1784" height="315" alt="image" src="https://github.com/user-attachments/assets/86714807-2290-4017-86df-7f42b4eb2f93" />

Oh my! Now so many words are obvious!! I won't point out each individual one, but rather, I'll make all the possible substitutions I see here.

y = y
b = s
h = u
w = h
s = l
x = g
z = d
i = k
d = w
f = v
m = b
a = q

<img width="1761" height="284" alt="image" src="https://github.com/user-attachments/assets/1d3c8430-8bc6-4ea7-a5d0-d3685467e24b" />

Aand, no more, since our flag is ready! Every letter in it has been replaced (bold = replaced) Let's put our flag in, and...

<img width="1452" height="728" alt="image" src="https://github.com/user-attachments/assets/e6ae21e9-9f86-4ea3-9991-a1aff535aa89" />

Neat!


