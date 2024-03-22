1. Step - Create a “Present Modally” segue between two ViewControllers 
   
   ![[Screenshot 2024-01-20 at 22.15.47.png]]

Hold Option key & connect Calculator View Controller to the Result View Controller.
Then you should see this menu:

![[Screenshot 2024-01-20 at 22.16.55.png]]


2. Click on "Present Modally"

Now you created the “Present Modally” segue between two ViewControllers.

3. Write an Identifier on the Present Modally segue

![[Screenshot 2024-01-20 at 22.18.47.png]]


![[Screenshot 2024-01-20 at 22.18.59.png]]
   
   
   Mine I called "goToResult"
   
   
   4. Go the the first Controller which is suppose to lead to the next view controller & write a performSegue command in order for transition to happen.
      
    Usually it is when the User press a Button which leads to another page.
    So here is my code:

![[Screenshot 2024-01-20 at 22.23.22.png]]

And the performSegue command which is the key for the transition to happen =>

![[Screenshot 2024-01-20 at 22.22.57.png]]


5. ![[Screenshot 2024-01-20 at 22.44.28.png]]


         