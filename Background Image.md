Setting Background Image for your App.

You can either go to the Main to design it or...


1. Prepare an Image and put it in the Assets ->
   
   ![[Screenshot 2024-02-24 at 0.28.22.png]]


here I prepared a few images just in case.

![[Screenshot 2024-02-24 at 0.28.34.png]]

2. ViewController -> ViewDidLoad() -> write the code:
   
   ![[Screenshot 2024-02-24 at 0.29.44.png]]


Code:

                // Create UIImageView
                
                **let** backgroundImage = UIImageView(frame: UIScreen.main.bounds)

                // Set the image

                backgroundImage.image = UIImage(named: "BGFibank01") // Replace "backgroundImage" with the name of your image asset

                // Ensure that the image scales correctly

                backgroundImage.contentMode = .scaleAspectFill

                // Add UIImageView to the view

                view.insertSubview(backgroundImage, at: 0)

3. Result
   
   ![[Screenshot 2024-02-24 at 0.31.39.png]]