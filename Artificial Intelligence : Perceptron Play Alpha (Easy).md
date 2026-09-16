In this space, I will be narrating my full experience with the Perceptron Play Alpha challenge.

Before we dive right in, think about it - a single perceptron has a boundary line that divides unaccepted and accepted inputs, right? It also finds the value via the w*x + b >= 0 and determines whether the input is acceptable or not based on whether the answer is greater than or equal to 0. I was thinking about perceptrons in general, until... wait... could this not all fit perfectly into a linear graph? I googled my theory, and...

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/319c2131-a0b6-462c-912a-c103552469e3" />

What do you know! On that note, here's the challenge :

<img width="1443" height="438" alt="image" src="https://github.com/user-attachments/assets/d9e8b408-cc55-4900-9124-b439309e44b0" />

Yeah, our challenge here also deals in two dimensions. And for two dimensions, the equation we have now is :

w1.x1 + w2.x2 + b >= 0

I found it simple enough. All we're doing is adding the second input, and naturally the weight is multiplied twice, since one set of input values can weigh different from the other, and the bias is chill. 
Well, let's begin!

Of course, the beginnings are always the same : 

<img width="422" height="26" alt="image" src="https://github.com/user-attachments/assets/bc9fe10d-ab02-427e-ac07-6326dddbe26b" />
<img width="702" height="686" alt="image" src="https://github.com/user-attachments/assets/67ad8f83-a21f-4dd5-a905-ff7625717e4a" />
<img width="335" height="197" alt="image" src="https://github.com/user-attachments/assets/08e7ad4b-8642-41e2-82ac-d36166f711c3" />


Oh man, that looks like a lot, huh? No matter. Alright, we won't confuse ourselves. Telling myself that, I started simple.
Again, we're still dealing with a single perceptron here. We'll use the good old methods, methods long before the descent of learning rates - trial and error.

<img width="368" height="502" alt="image" src="https://github.com/user-attachments/assets/0802840a-b227-4a23-98a7-c45302ac2fc9" />

Always remember, there's no need to overcomplicate things from the very beginning. Start from scratch, and if it's too simple to work, step up your algorithms a notch. I had all the time in the world to pull out a notebook and pen and start manually calculating everything, but I wanted to see if trial and error got me anywhere first. And I feel that this applies to all walks of life. Perceptrons, even. Test the waters to figure out how deep it is first. Or else you may end up diving straight into shallow waters and hit your head.




