In this space, I will be narrating my full experience with the Neuron Express 0 challenge.

Speaking of neurons, did you know that AI initially began with perceptrons? One perceptron basically simulates a neuron in your brain, and it denies and accepts certain inputs only. You could say a perceptron used to be a building block for AI.
They follow a specific equation too : w*x + b, where w is the weight of each input and b is the bias (the boundary line that separates acceptable and unacceptable inputs). And, naturally, x is the input itself.

So, on that note, this challenge is as follows :

<img width="1427" height="434" alt="image" src="https://github.com/user-attachments/assets/06f83346-e874-48dd-a253-3180962fa894" />

For now, we can only figure out the correct weights and biases via trial and error. Learning rates (that do it for us automatically) come later.
So, as such, this challenge took a considerable deal of trial and error.

<img width="404" height="30" alt="image" src="https://github.com/user-attachments/assets/4decafef-be97-41ff-a8b1-c819b08ecd09" />
<img width="713" height="210" alt="image" src="https://github.com/user-attachments/assets/45992543-eb27-4de5-8295-6a1a26b3d182" />

Of course, this is the easy part ; connecting to said perceptron in the first place.
Now, here comes the trial and error :

<img width="211" height="591" alt="image" src="https://github.com/user-attachments/assets/b3d05606-0821-4fb8-8c4b-f6a601a92645" />

It's certainly a primitive method, but hey, we're only dealing with a single, simple perceptron. The smaller the scale, the simpler the methods.
Based on my trial and error, as you can see in the image, the perceptron seems to accept any inputs that are 2 and above. So, I thought to myself, does that mean the boundary line is at 2? As for the weight, every input seems to be holding a weight of 1. It doesn't look like a single input needs to hold a weight greater than its own weight, especially since we're dealing with a single perceptron here with very simplistic methods. 
I decided to believe in Cylab Security Academy, thinking that they wouldn't be so petty so as to have the weight be greater than 1, since we're already dealing with input bounds of -10 to 10. Hey, it may not be the best method, but you gotta work smarter, not harder. With that, here we go!

<img width="484" height="36" alt="image" src="https://github.com/user-attachments/assets/241f3313-53a1-4487-a113-07e0de5cda15" />

...Oh. Well, this is awkward.
No, wait a minute, I get it! It's the bias! For a perceptron, the equation is w.x + b, but what I left out is the last part : w(x) + b >= 0.
A perceptron only fires (a 1) when the mathematical sum is greater than or equal to 0. So now, the way I understood the value of the bias is as follows :

w = 1, x = 2 (we need the decision boundary to be at 2, so the equation must equal 0/must equal the dividing line when x = 2)

w(x) + b = 0

1x2 + b = 0

b = -2

So just submit that, aaand...

<img width="273" height="58" alt="image" src="https://github.com/user-attachments/assets/4863329b-dbb5-448f-b2b3-8971c3163cd7" />

That's a wrap!



