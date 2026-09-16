In this space, I will be narrating my full experience with the Perceptron Train Hole in Middle challenge.

This, to me, was the most interesting part when completing the AI Foundations I - The Lost Book of Perceptrons learning path. The fact that it's never that simple and there's always a bigger fish. You'll see what I mean. 

Here's the challenge :

<img width="1449" height="421" alt="image" src="https://github.com/user-attachments/assets/de53e3b3-1090-4e39-befc-25fdf63b93c0" />

And so, I began.

<img width="426" height="25" alt="image" src="https://github.com/user-attachments/assets/4b8051f3-6d0e-466d-b204-0802b911ad02" />
<img width="1692" height="962" alt="image" src="https://github.com/user-attachments/assets/aa310b55-c843-468c-b322-4a7aa87fdfa9" />

So essentially, what I'm looking at here isn't news to me. Through previous challenges, I learned about learning rates, where you select a learning rate and a simulation is automatically ran to determine whether the weights and bias separate all the points perfectly or not. And the best part? It tells you how accurate you are in %, so none of that primitive trial and error anymore - you're no longer in the dark.

Now, I started simple with a 0.02... aaand...

<img width="1149" height="867" alt="image" src="https://github.com/user-attachments/assets/5872e800-53c5-4532-83d3-639dfc0fbd82" />

It seems I undershot. Let's try that again. How about we go really high? 20, perchance?

<img width="1151" height="858" alt="image" src="https://github.com/user-attachments/assets/92208693-951b-49ca-8425-938849ed0c03" />

And... we got it! But to me, this challenge was special, not because it was easy to get the flag, or because it took very little time to solve, no. I find this challenge particularly endearing because getting the flag isn't the focus, but rather, it's what I was taught here. 

Look at the image. It says we're only 88.9% accurate. Then, why'd we get the flag? It's because we're being taught that not all data sets are linearly separable, and hence, can never be 100% accurate.

Refer to the graph. We have an unaccepted point surrounded by accepted points, like the centre of a circle and its circumference. We're still dealing with a linear data set, and yet, when you look at it, there's no way you can separate both types of points with a single, straight line. You'd need a curved line, which goes into x squared territory, or, at the very least, two straight lines.

And this is where the bigger fish comes in. I learned that for anomalous data sets like these, one perceptron isn't enough. Throughout all of the AI Foundations I - The Lost Book of Perceptrons, i've been dealing with one perceptron, but that is but a drop in the ocean. To solve problems like these, you need a perceptron network. The fact that everything I was doing was all so tiny, so small in scale didn't make me feel powerless, but rather, it left me in awe at the scale of how much we humans can do and how much there is to learn and explore. And this left me with quite a sweet taste in my mouth. A single perceptron was the beginning for me, but it doesn't mean it's the end.


