# Dunder Methods
**Dunder methods** in Python are the methods having two prefix and suffix underscores in the method name. Dunder here means “Double Under (Underscores)”. These are commonly used for operator overloading.

## Enriching a Simple Account Class

- **Object Initialization: __ init__:** it is a reseved method in python classes. It is known as a constructor in object oriented concepts. This method called when an object is created from the class and it allow the class to initialize the attributes of a class.
- **Object Representation: __ str__, __ repr__:**
    1.  __ str__ is used in to show a string representation of your object to be read easily by others.
    2. __ repr__ is used to show a string representation of the object. In all honesty, eval(repr(obj)) is never used.
- **Iteration: __ len__, __ getitem__, __ reversed__:**
    1. __ len__: used to find the length of the instance attributes.
    2. __ getitem__: when used in a class, allows its instances to use the [] (indexer) operators.
    3. __ reversed__: eturns the reversed iterator of the given sequence.

- **Operator Overloading for Comparing Accounts: __ eq__, __ lt__:**
    1. __ eq__: Python automatically calls the __ eq__ method of a class when you use the == operator to compare the instances of the class.

    2. __ lt__:  describes the less-than operator 


- **Operator Overloading for Merging Accounts: __ add__:** used to add the attributes of the class instance.

- **Callable Python Objects: __ call__:** enables Python programmers to write classes where the instances behave like functions and can be called like a function. 

- **Context Manager Support and the With Statement: __ enter__, __ exit__:** 
    1. __ exit__: takes care of releasing the resources occupied with the current code snippet.
    2. __ enter__: allows you to implement objects which can be used easily with the with statement.
 
# Statistics - Probability

## What is probability?
**Probability** is the measure of the likelihood that an event will occur. This means that the probability is 0.5 (or 50 %) for both "heads" and "tails".

## The data and the distribution
The most important qualities to notice about the normal distribution is its symmetry and its shape. We’ve been calling it a distribution, but what exactly is being distributed? It depends on the context. In probability, the normal distribution is a particular distribution of the probability across all of the events. The x-axis takes on the values of events we want to know the probability of. The y-axis is the probability associated with each event, from 0 to 1.

<br>
In a probability context, the high point in a normal distribution represents the event with the highest probability of occurring. As you get farther away from this event on either side, the probability drops rapidly, forming that familiar bell-shape. The high point in a statistical context actually represents the mean. As in probability, as you get farther from the mean, you rapidly drop off in frequency. That is to say, extremely high and low deviations from the mean are present but exceedingly rare.

## Revisiting the normal
The normal distribution is significant to probability and statistics thanks to two factors: 
1. **Central Limit Theorem:** it suggests that if you ra n domly draw a sample of your customers, say 1000 customers, this sample itself might not be normally distributed. But if you now repeat the experiment say 100 times, then the 100 means of those 100 samples (of 1000 customers) will make up a normal distribution.
2. **The Three Sigma rule:**  dictates that given a normal distribution, 68% of your observations will fall between one standard deviation of the mean. 95% will fall within two, and 99.7% will fall within three. 

## Z-score
Z score is also called standard score. This score helps to understand if a data value is greater or smaller than mean and how far away it is from the mean. More specifically, Z score tells how many standard deviations away a data point is from the mean.   

    Z score = (x -mean) / std.

