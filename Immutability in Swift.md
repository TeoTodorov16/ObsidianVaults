In Swift, "immutability" refers to the concept of creating objects (like variables or data structures) that cannot be changed after they are initially set. Once an object is assigned a value, that value cannot be modified.

Swift was designed that anything mocked my the let keyword is immutable.

Suppose you create this structure =>

[![Amazing Lego Devices | Japan Style](https://lh3.googleusercontent.com/proxy/lc-xJWRIrAznNs5AqboGkcrs-uBvgSS9qp3JhZXC9bMmQo_Th16bgh_5RD8iTPh5WLV9xGyHvkFoCb8SvJdGKFeQVjcRZDYJMhBob0wEcjyKt3Q)


But at some point you decide that you want to change some aspect of it. Let's say the color of one of the bricks. Well unfortunately because the structure was created using the Let keyword - meaning it's immutable, you can't just change this one brick from green to yellow - Instead you have to destroy the entire structure and create a brand new one that has a yellow brick there instead.

The way I think about immutability is imagine if you created a sculpture of stone.

[![Is Michelangelo's 'David' really perfection personified? | Modern Healthcare](https://s3-prod.modernhealthcare.com/s3fs-public/David_WEB_edit.jpg)

If you created Michelangelo David and you decided it should have a larger nose, well you cant just come along and chip away at the stone because the nose is already too small. What you actually have to do is completely destroy this sculpture and create a new one with this gigantic ugly looking nose.


In summary, immutability in Swift means once you set a value using `let`, you can't change it. This can lead to safer and more predictable code.

Example:

<mark class="hltr-red">Error</mark>

![[Screenshot 2024-01-06 at 21.29.54.png]]


Fixing the <mark class="hltr-red">Error</mark>

![[Screenshot 2024-01-06 at 21.30.19.png]]


The fix is to add <mark class="hltr-red">mutating</mark> keyword in front of the function which is trying to change a self property inside of the structure 
             