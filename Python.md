

The first argument of every class method, including __init__, is always 
a reference to the current instance of the class. By convention, 
this argument is always named self. In the __init__ method, self refers to
the newly created object; in other class methods, it refers to the instance 
whose method was called.
