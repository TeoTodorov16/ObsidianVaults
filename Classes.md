I am going to explain about Swift Classes in this file.

what they are, what they can do, and how to create them...

![[Screenshot 2024-01-12 at 20.17.50.png]]


Now, classes like structures are, again, a way of defining a <mark class="hltr-blue">blueprint</mark>. They're a way for us to be able to plan our <mark class="hltr-red">properties</mark> and <mark class="hltr-green">methods</mark>. And eventually, when we run our app, be able to initialize our class into an actual object.


So how do we write the code for our class? Defining a class is very similar to defining a struct.

![[Screenshot 2024-01-12 at 20.25.29.png]]


We have the <mark class="hltr-red">class</mark> keyword and then we have the <mark class="hltr-blue">name</mark> of the class which is capitalized from the start, and then we have a set of curly braces inside of which we can define the implementation of the class.

________________________________________________________________________


Now Let's create a new class in another file called Enemy =>

![[Screenshot 2024-01-12 at 20.30.15.png]]


To create my class am gonna use the class keyword, and then I provide the name of my class which is going to be called Enemy.


![[Screenshot 2024-01-12 at 20.36.12.png]]



For the Enemy characters in my game, they might have a number of attributes or <mark class="hltr-cyan">properties</mark>. Things like, maybe they would have a health, stats, attack strength.

I can also describe behaviours that the enemies can perform.
So I would do that by creating a function.

Now that I've defined our blueprint that defines an Enemy character, it's ime to go into our main file where the code is & initialize my Enemy class there and create an object from that class.

Note:
![[Screenshot 2024-01-12 at 20.45.40.png]]

____

So in our main.swift, I'm going to create a new Enemy.

Let's say, it's a little skeleton and I'm going to initialize it as a new Enemy object,


![[Screenshot 2024-01-13 at 22.25.28.png]]

So I am printing the skeleton's health property.


![[Screenshot 2024-01-13 at 22.28.01.png]]

On the first line you'll see that the skeleton gets created on the second line I'm printing its health which turns

Now, in addition to using the <mark class="hltr-green">properties</mark>, I can also get my skeleton to do something, so I can write skeleton.move or skeleton.attack.

So now if I run my code, you can see that the health is printed as 100, the skeleton now walks forwards, it lands a hit and does 10 damage. Just by creating this Enemy class, I can now create lots and lots of enemies. I could create more skeletons, so skeleton2 is going to be created again from the <mark class="hltr-green">Enemy</mark> class.

![[Screenshot 2024-01-13 at 22.35.31.png]]

[![Waiting Skeleton Meme Generator - Imgflip](https://imgflip.com/s/meme/Waiting-Skeleton.jpg)

The magic of classes really lies within a special capability that they have which is the ability to inherit from a SuperClass.

So what do I mean by the SuperClass?

![[Screenshot 2024-01-14 at 18.28.27.png]]


We can have a relationships between classes.

Think of the SuperClass as a parent. It knows how to do certain things and has certain <mark class="hltr-green">properties</mark> and <mark class="hltr-red">methods</mark>.

![[Screenshot 2024-01-14 at 18.39.39.png]]

However, what if we want to take its existing capabilities and build on top of it?

Well, yeah, we could do this by adding more code to our existing class. But there's also another way. We can create a SubClass and add our additional functionality there.

Think of the SubClass as the child of the SuperClass. The SuperClass is taught the SubClass everything it knows how to do, for example, reading and swimming. And the SubClass can now grow and develop its own capabilities like playing with the iPhone, getting addicted to YouTube, or live streaming on Twitch.

![[Screenshot 2024-01-14 at 18.39.56.png]]


In other words, the SubClass has access to all the <mark class="hltr-green">properties</mark> and <mark class="hltr-red">methods</mark> of the SuperClass.

That's what we mean by <mark class="hltr-red">inheritance</mark>.


Lets Test this out:

Usually I had easy time destroying skeletons so why not creating something massive and hard to kill? What about a Dragon?

![[Screenshot 2024-01-14 at 19.08.06.png]]

Here I created a new File in the folder and gave it a name of Dragon

Then let's write some code in it ->


![[Screenshot 2024-01-14 at 19.07.50.png]]

This is the default way of creating a <mark class="hltr-red">class</mark> , whereas before I created a class that was just a simple standalone class.

In this case, I'm going to use the ability of classes to inherit from other classes.
Dragon is going to inherit from the Enemy class.

So that means when I create a dragon from the Dragon class, I don't actually have to redefine these properties or these methods.
It already has inherited all of those properties methods. And I can show you by simply going into my main.swift and create a dragon.

![[Screenshot 2024-01-14 at 19.13.05.png]]


So the dragon is gonna be created from the Dragon class.

And now with my Dragon class being completely empty other than the inheritance from the Enemy class, I'm going to use my dragon object, and I'm going to get it to move and I'm going to get it to attack.

![[Screenshot 2024-01-14 at 19.14.47.png]]


when this line 6 runs, the dragon walks forwards, and it also lands a hit when the attack method runs.

So without having to lift a finger, essentially, in our Dragon class, we've already managed to inherit all of the capabilities in the Enemy class.


Now that's not where it ends though...


The whole reason I created this Dragon class is for it to be able to do something different.

So let's create a property that is unique to our Dragon class. So maybe it has a wingSpan, and let's set it to default value of 2 meters.

So it's a medium-sized dragon.

![[Screenshot 2024-01-14 at 19.21.45.png]]


But when I create my dragon object, I could change that. So I could say dragon.wingSpan and let's set it to 5.
Let's make it a giant dragon.

![[Screenshot 2024-01-14 at 19.23.53.png]]


So this wingSpan property, of course, does not exist in our default sort of Enemy class.

I can't say skeleton.wingSpan. That doesn't make any sense. Skeletons don't have wings.
So that is a custom property that only exists inside the Dragon class.

But, of course, the Dragon class also has access to all the properties that the Enemy class has because it is inheriting from it.

![[Screenshot 2024-01-14 at 19.25.16.png]]

So, for example, it has the health property, it has the attackStrength property.

So let's set the attackStrength property to a bit higher than your average enemy.
Let's make it 15.

![[Screenshot 2024-01-14 at 19.26.27.png]]

Now, I also want my Dragon class to be able to do something that the default Enemy class can't do.

Now, it seems to me like from all the movies I've watched, dragons always seem to be able to talk. So let's give our dragon the capability of speech by adding a method code "talk," and this method is going to take a input code "speech", and that's gonna be a string data type, and then all that it's gonna do is just print the words it says whatever the speech happened to be.

![[Screenshot 2024-01-14 at 19.30.28.png]]


Back in my main.swift =>

![[Screenshot 2024-01-14 at 19.33.36.png]]

When I run my Program

![[Screenshot 2024-01-14 at 19.33.51.png]]


So you can see we've now got this dragon object created from the Dragon class which can do everything that the enemy can do, but it can do a lot more.

So there's some custom things that only the dragon can do that a bog-standard enemy can't.

One thing though... Shouldn't a Dragon fly instead of walk ?

So in addition to defining custom properties and methods, we can also tap into the methods that are available to us from the SuperClass, so the class that we're inheriting from, and we can override it.

![[Screenshot 2024-01-14 at 19.39.30.png]]

So if we tap into the move method, you can see that this override keyword goes in front of our normal function declaration.

And this means now that when we trigger the move method, we can say it does something completely different.

![[Screenshot 2024-01-14 at 19.41.40.png]]

In my case, I think that when a dragon moves, instead of walking, it probably should "fly forwards."


![[Screenshot 2024-01-14 at 19.42.54.png]]

So now if I go back to my main.swift without changing any of this code, I run my code, you can see now when my dragon moves, it flies forwards, instead of walking forwards. And I've managed to achieve that by overriding this method that I got from my SuperClass and providing a custom implementation, so doing something completely different from the move method that the dragon inherited.

________________________________________________________________________

Now sometimes, however, you actually want the behaviour of the method from the SuperClass.
So in our case of our dragon, what if I want it to land a hit, do some damage, but also to maybe be able to spit some fire, in addition.

I can override the attack method from my SuperClass and I can do something customised to the Dragon class.

![[Screenshot 2024-01-14 at 20.01.00.png]]
I want it to perform the method that came from the SuperClass, the Enemy class, which I'm inheriting from, but then do some custom stuff as well.

So I want both the functionality of the attack method from the SuperClass, as well as some functionality that I've added on as custom.

So to achieve this, what I do is I use the super keyword which refers to the Enemy class which I'm inheriting from, and then I write "<mark class="hltr-blue">.attack</mark>." ->

![[Screenshot 2024-01-14 at 20.02.25.png]]

So now I'm triggering the attack method from my SuperClass which will print "Land a hit, does X amount of damage," and then I want to "<mark class="hltr-orange">Spits fire and do an extra 10 damage.</mark>"

![[Screenshot 2024-01-14 at 20.05.20.png]]


You can see that by inheriting from the Enemy class, I saved myself a lot of work and a lot of repetition.

When we create functions, we know that they help us reduce the amount of repeated code by packaging a whole bunch of instructions inside the same package.

Now, when we create classes and inherit from other classes, we're, again, saving ourselves from creating repeated bits of code and instead, we are just layering functionality upon a SuperClass.

This is called - <mark class="hltr-red">DRY</mark>

Which is not repeating yourself and maintaining less code as possible.

Last thing before I finish this Documentation about classes:

![[Screenshot 2024-01-14 at 20.08.31.png]]

Going on "Help" -> "Developer Documentation"

 You can see how inheritance is used amongst the components that are part of Apple's UIKit. And that includes almost everything we've shown on screen like UILabels, UISliders, UIImageViews, everything with a UI in front of it, basically.

![[Screenshot 2024-01-14 at 20.13.18.png]]

So for example, when we create a button, we're actually creating a UIButton.

![[Screenshot 2024-01-14 at 20.19.34.png]]

![[Screenshot 2024-01-14 at 20.19.57.png]]

So if you search for a UIButton and click on it, you can see that this is a UIButton Class and it allows you to respond to user interactions. But this class actually inherits from the UIControl Class.


![[Screenshot 2024-01-14 at 20.28.43.png]]


So when I click on UIControl, we get taken to this class' documentation and you can see that this is the base class for all of the controls which convey a specific action or intention in response to user interactions.

![[Screenshot 2024-01-14 at 20.34.03.png]]


![[Screenshot 2024-01-14 at 20.34.18.png]]


![[Screenshot 2024-01-14 at 20.34.35.png]]

So we're inheriting some of these capabilities when we use a UIButton. Now, a UIControl itself then inherits from a UIView which is an object that manages the content for a rectangular area on the screen. And then a UIView itself inherits from UIResponder, and UIResponder inherits from NSObject.


So what does that mean?

Why is it structured like that?

Well, let's think about it in reverse.

Apple's most basic class is the NSObject.

This is the simplest and most generic component.

And it's how Apple started out. The NS, in fact, stands for NeXTSTEP which was the company that Steve Jobs started when he got kicked out of Apple, initially.

[![Apple II manual signed by Steve Jobs auctioned for $800,000](https://www.usatoday.com/gcdn/-mm-/235e72b0e08a1b2da71b731c693e4f0282bfa8cb/c=46-0-533-649/local/-/media/2019/01/09/USATODAY/usatsports/MotleyFool-TMOT-467f57f7-a0347979.jpg?width=487&height=649&fit=crop&format=pjpg&auto=webp)


Now, the UIResponder can do everything an NS object can do, but it has its own additional capabilities. The UIView in turn builds on top of the capabilities of the UIResponder, and the UIControl builds on top of that again. At each level more code and more capabilities are added so that components become less generic and more specialised.

![[Screenshot 2024-01-14 at 20.42.42.png]]

Until finally, we get a UIButton that the user can press. So now that we've chased it all the way up the tree, we can see how it would take so much longer if we had to create everything from scratch, and create all of our view controllers from scratch, all of our UILabels from scratch, rather than simply just inheriting and using the capabilities that <mark class="hltr-grey">Apple</mark> has already created within our UIKit.

       