Design Patterns in Coding is what helps us get organized & structure our code in a better way.

![[Pasted image 20240107193702.png]]


Design Patterns is a proven solution to a common problem.
With Software that problem is usually complexity.


It's like having a Restaurant

![[Pasted image 20240107193803.png]]


A restaurant full with clients would be a mess for a one person to cook and serve.
And most people think what is going to fix the problem is hiring more staff.

Well...

That is not quite the solution

![[Pasted image 20240107195513.png]]


A restaurant full of staff who don't know what they are doing would be complete mayhem

![[Pasted image 20240107194512.png]]


Don't ask me from where I know...

The best restaurant have staff who knows exactly what they are supposed to do at any given point. 
In short a restaurant have specialist over any area in the cooking Industry 🧑‍🍳 

And it's the same thing managing complexity everywhere.

Companies have a lot of complexity and so do software

No there are many many Design Patterns to existing and everybody have different opinion on which one is the best pattern 

However we have to remember, just like in life - There is not such thing as the one best ULTIMATE Design patter that you should learn and always use and never think about any of the other ones.

Because at the end of the day a Design pattern is something like an Architectural BluePrint

IMAGE

Depending on what Project you are working you might use different Design Patterns 


For some programmers, they want to have as <mark class="hltr-red">FEW</mark> lines of code as possible and others as <mark class="hltr-yellow">READABLE</mark> as possible.


<mark class="hltr-red">IMPORTANT!</mark>
The most fundamental Design Pattern that Apple chooses to use

MVC (Model View Controller)


![[Pasted image 20240107200055.png]]

We split the project to 3 main components:
- Model
- View
- Controller

And by making those 3 components work together we end up with the MVC Design Pattern.


Let's say you have a big successful app in the App Store that users are demanding a version in German, French, others want a history version or a science version then you won't actually need to touch the controller or the view.

All you need to modify in order to change the app for this purpose is to <mark class="hltr-red">switch out the Model</mark>
You might need to change the logic a little bit or you might need to update the data. 
But you won't need to go into the ViewController.swift file or the Main.Storyboard where the main design files are.


So it all makes reduce errors and be EASIER to understand especially for other programmers who know the MVC.

![[Pasted image 20240107195942.png]]



    