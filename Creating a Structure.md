
1.

<mark class="hltr-purple">struct</mark> <mark class="hltr-green">MyStruct</mark>  {           }

<mark class="hltr-green">MyStruct</mark> ( )



Now this is a structure I wrote in myPlayground in Xcode 

Full Code

    struct Town {
    
    let name = "Teodorland"

    var citizens = ["Angela", "Teodor"]

    var resources = ["Grain" : 100, "Ore": 42, "Wool" : 75]
    
    }

![[Screenshot 2024-01-03 at 15.29.33.png]]


2.Now second thing I am going to do is create an Object that I can use

![[Screenshot 2024-01-03 at 15.34.57.png]]


Now this is going to be the actual Town created from my Structure

![[Screenshot 2024-01-03 at 15.36.04.png]]


So now what is happening is I created a new copy of this <mark class="hltr-green">Town()</mark> structure and its held within the variable of <mark class="hltr-cyan">MyTown</mark>.

That means I can actually use this object <mark class="hltr-cyan">MyTown</mark> and I can access the properties of <mark class="hltr-cyan">MyTown</mark>

![[Screenshot 2024-01-03 at 15.44.34.png]]


Now let's say I want to Add something into my structure by accessing it again through my 
<mark class="hltr-cyan">MyTown</mark>

![[Screenshot 2024-01-03 at 15.58.00.png]]

I access the citizen property of <mark class="hltr-cyan">MyTown</mark> so I can append/add something into my citizens array  and the name I am going to pend is my neighbour Keanu Reeves from work.

And when I print it with using <mark class="hltr-purple">.count</mark> =>
We can see 3 - as 3 people living now.

________________________________________________________________________

Now watch this =>

![[Screenshot 2024-01-03 at 16.16.14.png]]



Full Code 

    struct Town {
    
    let name = "Teodorland"

    var citizens = ["Angela", "Teodor"]

    var resources = ["Grain" : 100, "Ore": 42, "Wool" : 75]

    func fortify() {

        print("Defences increased!")

    }
    
    }


The function <mark class="hltr-blue">fortify() </mark> inside the structure. 
When a Function is inside a structure it is called a <mark class="hltr-red">Method</mark>


If a functions is free floating around outside of the structure is just a normal function.

Now I can trigger this Method that <mark class="hltr-cyan">MyTown</mark> has by ->

Writing <mark class="hltr-cyan">MyTown</mark> which is the actual Object that can do things and has properties 




![[Screenshot 2024-01-03 at 16.22.17.png]]



Also here we can clarify the function is a method in the structure that the variable/Object is using.

![[Screenshot 2024-01-03 at 16.25.07.png]]


________________________________________________________________________

3.Initializing 


Now this whole thing of creating a structure and using objects to access it's properties is just a <mark class="hltr-blue">BluePrint</mark> 
And we can take our <mark class="hltr-blue">BluePrint</mark> and Initialize it which turns it into the actual object.

Here is what I mean:

![[Screenshot 2024-01-03 at 17.32.36.png]]

Just like we create a function we create our Initializer in a pretty similar way.

The Initializer gets triggered when we create our object from our BluePrint.

For instance when we create next Civilization like me (It's quite difficult just so you know)

![[Screenshot 2024-01-03 at 17.34.35.png]]


In that case you need more than just one Town.
So all those places are different from each other in their own way.

They have different name, different citizens, and different resources.

So what if we use our struct to act as a BluePrint for all new Towns but still be able to customise each Town.

<mark class="hltr-red">That's where the Initializer comes in!</mark>


![[Screenshot 2024-01-03 at 18.46.09.png]]

I just deleted the values of these properties to keep it very generic.
So now my Town structure has blank properties for each of this attributes - Now I can define a custom property every time I create a new <mark class="hltr-cyan">Town</mark>.

Before that I need to create the Initializer: 


![[Screenshot 2024-01-03 at 18.51.26.png]]

When I start to type it, it gives me this code snippet and notice how it's made in as it gives all of the parameters by default. It recognise the structure that is in.

Hit Enter

![[Screenshot 2024-01-03 at 18.54.04.png]]

Edit(Explaining the <mark class="hltr-red">self.</mark>  [[the Self keyword in Swift]])

now I am going to edit the code a bit 

![[Screenshot 2024-01-03 at 18.57.05.png]]

________________________________________________________________________

Now lets say I create variable called anotherTown

![[Screenshot 2024-01-03 at 19.00.54.png]]

Here I am using the structure <mark class="hltr-cyan">Town</mark> as a BluePrint again and notice how since opening the first bracket it gives all of those input parameters show up.

Hit Enter

![[Screenshot 2024-01-03 at 19.02.28.png]]

Now using Tab you can move between those.

Now I need to <mark class="hltr-red">provide some values to these positions</mark> 
We also see what type of data I need to provide.

here I made two =>

![[Screenshot 2024-01-03 at 19.38.34.png]]


and all using the <mark class="hltr-blue">BluePrint</mark> <mark class="hltr-red">structure</mark> <mark class="hltr-blue">Town</mark>

       