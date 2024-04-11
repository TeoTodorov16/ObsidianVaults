
![[Screenshot 2024-02-16 at 23.40.59.png]]


The very first London Underground was built in 1863 which is actually crazy if you think about it.

That was like the time of horse and carriages. But, okay, maybe a little bit later than that.

Imagine that if you build an underground or a train line, it's pretty likely that as your city grows,
you're going to have to add extra lines, extra stations, and extend the train line.

So this is kind of similar to how Swift extensions work. Extensions, essentially, allow us to add extra functionality to our existing classes, structures, or other data types.

And so that means if you build a project and it was really, really great, but then your boss comes along and says, 

"Actually, you know what we need to do for the next quarter, we need to add all of these extra capabilities." 

![[Screenshot 2024-02-16 at 23.44.26.png]]

Instead of diving into the original code and ripping bits out and switching things around, we can simply just extend the functionality of our existing code. So the way that we would create an extension would be something like this. ->

![[Screenshot 2024-02-16 at 23.45.27.png]]

We would have the extension keyword, and then we can have the name of an existing type, so that could be a class, that could be a struct, that could even be a protocol.

And then inside the extension, we would get to add some new functionality to that type. 

Here is an Example:

![[Screenshot 2024-02-21 at 12.07.35.png]]

the <mark class="hltr-blue">UIButton</mark> is what we get from the library UIKit.

Then I make a method called <mark class="hltr-cyan">makeItCircle()</mark> and set a new functionality for making an object into a circle.

<mark class="hltr-red">self.</mark> - represents the object that is going to use the method <mark class="hltr-cyan">makeItCircle()</mark>.

Then it enters into the properties of a <mark class="hltr-blue">UIButton</mark> such as <mark class="hltr-purple">clipsToBounds/layer/cornerRadious/</mark> & set the value to be the self. (meaning the object that is going to use it) -> properties of the object that are suppose to be written. 

Then I set the color of the button variable constant to be red. 
Lastly I implement the method to the button since it's using the UIButton library.
                   