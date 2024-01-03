
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


2  Now second thing I am going to do is create an Object that I can use

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

