# Decorator-design-pattern-project


Decorator design pattern : A Decorator pattern can be used to attach additional responsibilities to an object either statically or dynamically. A Decorator provides an enhanced interface to the original object.

In the implementation of this pattern, we prefer composition over an inheritance – so that we can reduce the overhead of subclassing again and again for each decorating element. The recursion involved with this design can be used to decorate our object as many times as we require.


PROJECT PROBLEM

Definition
We are creating a restaurant menu design, in which we are prompting the user to choose an item from menu. The food he orders might also contain combinations of different food items. Finally we have to calculate the total cost of the food items that is selected by the users.
Problem occurred
If a person choose a food item that contains a combination of two or more items
Then there was a need to create a different class to represent that item.
Problem Solution
To get the cost of combination of different items , its not necessary to create a new class of that particular items but we can decorate it dynamically with the suitable items.


JUSTIFICATION

The design pattern which we will use to solve this problem is Decorator pattern.
In decorator Pattern, we can add responsibilities to individual objects dynamically and transparently, that is, without affecting other objects.
In this particular example, There was no need of creating different functions for the combined items selected by the user. From the definition of Decorator pattern , we can know that , we can create each classes dynamically for different item .
In this scenario if a person chooses a Veg item then the cost will be normal , but if a person chooses a Non veg item or a Chinese food item then there will be change in the cost , as this particular food items comes with the inclusion of Veg food item. If the user choose the food items that contain more than one item , then we have to show the cost of both the food items. Then the implementation of this gets complex ,as we are creating a class with cost of both the food items. 
Imagine if we have 4-5 items in a single food item , then it might get more complex for implementing this. To solve this kind of problem we can only use decorator pattern.
