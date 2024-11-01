## Lists

- Ordered and mutable collection
	- Can add, remove, or modify elements
	- Mutable = Changeable
- You can have any type of data in a list
- Used when data may change over time
- Accessed **by index**

```python
# List of sites to hold SCPs
containment_sites = ["Site-19", "Site-17", "Area-14"]
containment_sites[1] = "Site-21" # This code works
containment_sites.append("Site-13") # Adds an item to end of the list
containment_sites.remove("Area-14") # Removes an item with the argument's value
print(containment_sites) # ['Site-19', 'Site-21', 'Site-13']
```

- Defined with **square brackets** []
- Use when data needs to be **modified frequently**.

## Tuples

- **Ordered** and **immutable** collection.
	- Cannot add, remove, or modify elements
- Defined with **parentheses ()**
- Used when data that should remain constant
* Good for **fixed categories** or statuses
* Accessed **by index**
* If a list is in a tuple, **you can use list methods on the list, not the tuple.**

```python
# Tuple holding classifications of SCPs
# Object classes are tuples because they are astandard and should remain unchanged. 
# This data will remain consistent throughout the program.
object_classes = ("Safe", "Euclid", "Keter", "Thaumiel", ["Fuck!??"])
object_classes[2] = "KETER" # This code does not work
print(object_classes[-1]) # Prints the last value in the tuple
object_classes[4].append("Shit!??") # Appends to ["Fuck!??"]
print(object_classes)
```