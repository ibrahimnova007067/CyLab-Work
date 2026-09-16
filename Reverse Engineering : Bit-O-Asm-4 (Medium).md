In this space, I will be narrating my full experience with the Bit-O-Asm-4 challenge.

Truthfully, unlike virtually every other CyLab Academy challenge, I'm familiar with this set of challenges (Bit-O-Asm) due to the fact that I studied Assembly Language in great detail in my AS Level in Chapter 4. So, this is how I broke it down :

<img width="766" height="258" alt="image" src="https://github.com/user-attachments/assets/28eda2d8-54c3-4ccb-9303-f4894ea6e694" />

 When we open up the file, we see this : 

<img width="462" height="306" alt="image" src="https://github.com/user-attachments/assets/9be95531-12ee-4473-9a7c-19cd6107b02a" />

Wow, that looks incomprehensible, but it's actually simple. A bunch of this is just noise, and we only need to focus on what's important.
At +41, the value at DWORD PTR [rbp-0x4] is being moved into eax, so we only look at key commands and commands related to our DWORD PTR [rbp-0x4] here.
I see only one key command, and that's jle here. I knew this was a jump instruction by the first letter, but I didn't know the conditions. After a quick Google search as a refresher, this stands for "jump if less than or equal to". We'll leave that there for now.

<img width="448" height="43" alt="image" src="https://github.com/user-attachments/assets/7086627e-ac5e-4509-93ec-f06bcb386e42" />

These are the only two instructions related to before our 'jle', so let's see here...
<+15>: Simple enough - the value '0x9fe1a' is being moved into DWORD PTR [rbp-0x4]
<+22>: cmp stands for 'compare'. We're comparing the value inside DWORD PTR [rbp-0x4] (0x9fe1a) with 0x2710. Let's do a quick conversion, and...

<img width="130" height="536" alt="image" src="https://github.com/user-attachments/assets/6e23feec-92bf-4dbd-b267-ae522d7827a3" />
<img width="125" height="536" alt="image" src="https://github.com/user-attachments/assets/1e80c072-eabd-4ece-a1f7-3f10926e620e" />

Oh wow, that... isn't even close.
Well, after that brutal comparison, we're immediately followed up by our main culprit - 'jle'

<img width="422" height="21" alt="image" src="https://github.com/user-attachments/assets/46f0ced9-53b0-4dd8-9b2d-62d341a816ba" />

<+29>: Yeah, that's not gonna jump, so we proceed as usual. Now, looking at the instructions AFTER our 'jle' :

<img width="434" height="92" alt="image" src="https://github.com/user-attachments/assets/4a40ceb5-eba5-4c2f-a0ec-27a4aa4b1ea9" />

<+31>: Here, because it says "sub", we're subtracting 0x65 from 0x9fe1a. Using CyberChef yet again, that gives us :

<img width="134" height="531" alt="image" src="https://github.com/user-attachments/assets/d60c68ee-4bb9-4aca-8caf-1f2a41ac2709" />
654874 - 101 = 654773

<+35>: That's just an unconditional jump. Hey, I'm not complaining ; makes things easier for us.

(We skip <+37> because of the jump.)

<+41>: So now, eax comes out to a value of 654773, and that's our answer... hopefully...

<img width="1440" height="648" alt="image" src="https://github.com/user-attachments/assets/3f268110-891f-4359-b5bf-63f2489a6a20" />

Alright!

