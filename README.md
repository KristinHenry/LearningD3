LearningD3
==========


Important concepts: Data Binding, Method Chaining, ...


Data Binding
------------

If you're experienced with looping through data sets, and writing code to process that data directly, D3's Data Binding may be a little tricky to wrap your brain around. You may find that you're looking for the loop. But you have to let go of the loop, and let data binding run the loop for you. Yeah, it's a little weird.



Method Chaining
---------------

This one is easier. Basically, an object's method returns a modified version of the object itself?  If you're used to coding getters and setters, you'll have to let go of that. In method chaining, the same method does both getting and setting. You need to test for input parameters. If there is input, you return the modified object. If not, you return the value of that property of the object. 
