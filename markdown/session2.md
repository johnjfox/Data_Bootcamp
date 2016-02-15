#### Session 2 

**Prelaunch checklist**
* Start Spyder
* Locate this document (Google "nyu data bootcamp", look for mini-course link)
* Save code files, open them in Spyder 

**Review.**  Sketch brief answers.  Feel free to consult your neighbor. 

Concepts.  Explain each of the following:   
* `x = 107.3`
* `x = x**2` 
* `'this'` and `"this"` 
* `y = '3.14159'`
* `y = 2 * y`
* `float(y)` 
* `z = [3, 2, 7, 2]`
* `type(x)`
* `type?`
* `w = z.count(2)` (This one's harder; the idea is to use the available help to find out what it does. Or just try it.) 

Problems.  
* What should you do if you don't follow what we're doing in class?  
* Set `first = 'Hersh'` and `last = 'Iyer'`.  Construct a string `bothnames` that consists of the first name, a space, and the last name in upper-case (capital) letters.  
* Suppose we have a variable `z = '12,345.6'`.  What is its type?  Can we convert it to a floating point number?  (This one's harder.  Hint:  What method can we use to get rid of the comma?)  

Reminders:  IPython console, Object explorer, code cell 

**Data and graphics** 

Packages 
* Packages/libraries/modules = plug-ins that add new tools to Python 
* There are lots of them
* Our favs:  Pandas (data), Matplotlib (graphics)
* The `import` command

Data basics 
* `import pandas as pd` 
* Reading spreadsheets and csv files 
* Dataframes:  column labels, row labels, dtypes, ...   
* Internet sources with APIs:  FRED, World Bank, Fama-French  
 
Graphics basics 
* `import matplotlib`
* Approach 1:  `plot(x,y)`
* Approach 2:  apply methods to `fig, ax` 
* Parameters and styles 
* Approach 3:  apply `plot` method to dataframe 

Examples 
* GDP in various countries
* Emerging market indicators 
* US GDP and GDP growth 
* Indicators of US economic conditions 
* US stock returns 
* Healthcare spending 

**Graphics practice.** 
Randy Olson has a
[nice blog post](http://www.randalolson.com/2014/06/28/how-to-make-beautiful-data-visualizations-in-python-with-matplotlib/) (or Google "randy olson beautiful") about creating effective graphics.
He starts with [this gif](http://gfycat.com/ImprobableFemaleBasenji).
Skim his post, play the gif, and
* Write a Python program that recreates the data in the figure, both numbers and labels.
(There are only a few points, you can just type them into lists.)
* Approximate the various graphs using Matplotlib.
* Play around with the graphics parameters.
What is the best graph you can produce?
What do you like about it?
* Variant:  Do the same with our GDP per capita bar charts.

If you'd like to do more of this on your own:     
* Browse the [Practical Business Python](http://pbpython.com/) blog, it's filled with practical information about how to go between Pandas and Excel.  Start with [this one](http://pbpython.com/excel-pandas-comp.html).
* Watch Brandon Rhodes's [video](https://youtu.be/5JnMutdy6Fw), it's a wonderful start on advanced features of Pandas.  Two hours long, but worth it.  
* Check out the Matplotlib [gallery](http://matplotlib.org/gallery.html) of examples, they all come with code you can run yourself.  
* Wait till we write the relevant chapters of our book.  

**Mailing list.**  If you'd like to get announcements about similar events, sign up for the NYU Data Bootcamp [Google Group](https://groups.google.com/forum/#!forum/nyu_data_bootcamp).  

A product of the #nyuecon Python factory 