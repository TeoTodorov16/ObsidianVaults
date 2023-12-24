
So I make a new App called EggTimer:
![[Screenshot 2023-10-10 at 20.21.57.png]]

Now My first step is to set all of the buttons with the images (eggs) under 1 single IBAction.

This is the following steps:

1. Open the View Controller

![[Screenshot 2023-10-10 at 20.24.26.png]]

2. Create one IBAction from whatever button you choose

![[Screenshot 2023-10-10 at 20.27.35.png]]

Then Select on <mark class="hltr-grey">Connection</mark> : <mark class="hltr-red">Action</mark>
   	                 <mark class="hltr-grey">Type</mark> : <mark class="hltr-red">UIButton</mark>

Then the code should look something like this:

![[Screenshot 2023-10-10 at 20.30.56.png]]


3. Now Adding the other Buttons to the same IBAction

You can drag the Action to connect with the button by dragging it form the + 

![[Screenshot 2023-10-10 at 20.31.34.png]]

4. Checking if it's Correct


![[Screenshot 2023-10-10 at 20.33.40.png]]
When you hoover the mouse on the plus sign, if it covers all of the eggs with blue like the example then they are selected which means they are all under the single IBAction.

5. That's it.



<mark class="hltr-red">Extra</mark>

If you want to trigger each one of the buttons and print different outcomes individually ->


![[Screenshot 2023-10-10 at 20.42.20.png]]


<mark class="hltr-grey">sender</mark> is the button that triggers the <mark class="hltr-pink">IBAction</mark> and then we  select one of his properties which is the <mark class="hltr-purple">currentTitle</mark>

Output:


![[Screenshot 2023-10-10 at 21.05.18.png]]

And this is the outcome of selecting each of the buttons individually
