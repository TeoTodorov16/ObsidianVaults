# Changing the text of UIButton programmatically in Swift

![[Screenshot 2024-01-07 at 22.31.40.png]]


So I found how to do this in StackOverflow.

You firstly target the name of the IBOutlet that the button is connected to and access it's property of <mark class="hltr-purple">setTitle</mark>.
Then you can either type a string as following <mark class="hltr-orange">"Take a left."</mark> or straight adding the name of the variable/constant that points to the wanted string.
Then the <mark class="hltr-purple">for: .normal</mark>  - The titles are set for the normal state of these buttons. The normal state is the default state that a button is in when it is not highlighted or disabled.

Conclusion:
In Swift, the `for` parameter in the `setTitle(_:for:)` method is specifying the control state for which the title should be set. The `.normal` state is the default state for many UI controls, including buttons. It represents the normal, unhighlighted state of the control.

