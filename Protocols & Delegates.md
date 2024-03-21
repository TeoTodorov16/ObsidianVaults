Section 13 - 147

Explain that later



The SuperClass needs the Delegate (as property) which is of DataType - Protocol. [Doesn't need to know who the delegate will be - either a class or structure, it cares only as long as they have the Protocol which is basically the rule in order to be the delegate]
SuperClass -> Delegate


SubClass needs only the Protocol
SubClass -> Protocol
[Subclass becomes the Delegate and in order to be one you need the Protocol as DataType]
-> Must perform whatever method is in the Protocol in the SubClass
+set the superclass as the delegate(to inform that the superclass is the original delegate) = weatherManager.delegate = self
  