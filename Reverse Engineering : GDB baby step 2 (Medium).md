In this space, I will be narrating my full experience with the GDB baby step 2 challenge.

Yet another useful tool known as GDB was added to my collection with the GDB baby step series, and of all the GDB challenges, GDB baby step 2 felt the most informative and useful to me, because it brought to life and actual practice something I studied in AS Computer Science Chapter 5 : Breakpoints.

Here's what we're gonna tackle :

<img width="1396" height="358" alt="image" src="https://github.com/user-attachments/assets/65430b56-4223-4be5-9cad-de545fd8e73e" />

Now, it all starts with... wget. It always did, always does, and always will.
Alright, what I've learned about is this neat little tool in our webshell called GDB. To activate it for a certain file, we'll use :

<img width="624" height="369" alt="image" src="https://github.com/user-attachments/assets/3d6b6572-f8c9-4b25-9e81-ee868ca83396" />

But, what we care about is the fact that we can use gdb to disassemble the program and fully view the assembly code inside of it as follows :

<img width="478" height="422" alt="image" src="https://github.com/user-attachments/assets/dd33b1de-27fc-4c72-953c-43175ab0293b" />

Those are a lot of words, huh? But first, let's just try simply running the program and see if it works or gives us some sort of error.

<img width="615" height="175" alt="image" src="https://github.com/user-attachments/assets/fb72d16e-1f98-4e37-a887-eb7c6f049972" />

Hmm, look at that. It seems that after the program is finished, we can't inspect final register values. If we were able to, we would've directly gotten the answer, so how do we solve this?
Ashamedly, I have to admit that I hit a dead end and decided to open a hint. But I did a ton of stuff perfectly until this part, okay?!

<img width="1269" height="97" alt="image" src="https://github.com/user-attachments/assets/47fadc76-19ed-403b-9633-6ac130277fb3" />

Set a breakpoint... Yeah, that would fix it! When we set a breakpoint, code execution stops when that point is reached but the program doesn't fully finish because there's still stuff to execute AFTER the breakpoint, and what I'm noticing here...

<img width="287" height="25" alt="image" src="https://github.com/user-attachments/assets/7b95fea3-f7c6-470c-a98c-866dad5b38ef" />

This part is pretty useless for us! So what if we set a breakpoint such that the entire program has ran except this SINGLE instruction! And then we can inspect our register safely. So... uh... how do we set a breakpoint?

<img width="175" height="24" alt="image" src="https://github.com/user-attachments/assets/ca824b83-e375-4c37-a4c8-a4463062c8c9" />
Ah, found it, so let's do our thing now, and...

<img width="627" height="756" alt="image" src="https://github.com/user-attachments/assets/ead90c29-84ce-4bde-9ac6-24666646c8ee" />
<img width="1439" height="662" alt="image" src="https://github.com/user-attachments/assets/d4fe635e-e826-433c-8bcc-c018f2d70e08" />

Sweet!


