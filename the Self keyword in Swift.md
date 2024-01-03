Heyo! 

As example I am going to use the Swift structure from the current Project 
[[Creating a Structure]]

![[Screenshot 2024-01-03 at 19.22.28.png]]

Notice how I am twisting these names so that they overlap with the names of the properties I have.

It's easy to do them like this:

![[Screenshot 2024-01-03 at 19.23.54.png]]


Xcode doesn't even allow it.

This code on the other hand is veery confusing, right?
The other Engineer is gonna try to connect which is what here. (wethers the property or the input there)

And that's where the <mark class="hltr-red">.self</mark>  comes into hand.

![[Screenshot 2024-01-03 at 19.12.40.png]]

It refers to the Eventual object that will be created from this structure <mark class="hltr-blue">BluePrint</mark>

where we say <mark class="hltr-red">self.</mark><mark class="hltr-green">name</mark> referring to the property name of the structure <mark class="hltr-blue">Town</mark>

So this <mark class="hltr-red">self.</mark> is referring to the structure.

