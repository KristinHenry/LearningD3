LearningD3
==========


Important concepts: Data Binding, Method Chaining, Scale...enter/exit?


Data Binding
------------

If you're experienced with looping through data sets, and writing code to process that data directly, D3's Data Binding may be a little tricky to wrap your brain around. You may find that you're looking for the loop. But you have to let go of the loop, and let data binding run the loop for you. Yeah, it's a little weird.



Method Chaining
---------------

This one is easier. Basically, an object's method returns a modified version of the object itself.  If you're used to coding getters and setters, you'll have to let go of that. In method chaining, the same method does both getting and setting. You need to test for input parameters. If there is input, you return the modified object. If not, you return the value of that property of the object. 


D3.Scale
---------
This is a very handy feature of d3.js. You can use it to convert data values into relative positions in a chart. It takes care of figuring out what pixel position a data point would be.

First, you set up your scale with the **domain** (min, max values in your data set) and a **range** (min,max in your chart). 

So, if you had a data set of [100, 116, 302, 489] and you wanted to map that onto a chart 20x80 pixels in size, you could create this scale.

`var scale = d3.scale.linear()
                    .domain([100, 500])
                    .range([20, 80]);`
                    
  
  
Then, for each data value you want to draw, you use scale(datavalue).

                    
`scale(100);  // returns 20`





