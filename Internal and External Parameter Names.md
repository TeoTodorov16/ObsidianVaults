

![[Screenshot 2024-02-13 at 13.00.45.png]]

<mark class="hltr-red">Important!</mark> 
In the predecessor to Swift, Objective-C, which used to be the language that we used to make iOS apps, they weren't really big on parameter names.

Instead, you ended up with really, really long method and function names to describe exactly what the function is supposed to do. But in Swift, it's meant to be about well-named parameters that clearly describe the functionality.

And this ability of Swift methods and functions, to be really clear, relies really heavily on a particular feature of the Swift parameter names.

And it's the ability to have completely separate internal and external parameter names.

So in this case, instead of having a single parameter name, the word "name," we now have a external name which is the name that will refer to the parameter when we call the function, and an internal name which is the name that we'll use when we need to use the parameter within the function.

![[Screenshot 2024-02-13 at 14.15.16.png]]


So in this case, the external parameter name is what we're using when we call the function, and the internal parameter name is what we use when we need to use the value of that parameter within the function.


![[Screenshot 2024-02-13 at 14.17.04.png]]

Now, you can also if you wanted to, actually omit the external parameter name altogether to be able to call your function just by passing in a value without mentioning the name of the parameter at all.

So how would we do that?

Well, all that we would need to do is simply turn the external parameter name into an underscore.
And now we can call our function without using a parameter name at all.

And instead, all we have to do is just pass in the value that we want to use as the input.

![[Screenshot 2024-02-13 at 14.19.51.png]]

So in this case, we still have an internal parameter name which we can use to refer to the value within the function.

But when we call the method, we no longer have an external parameter name.
          