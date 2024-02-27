# Numpy
This repo contains the basic python files, that is a practice files of Numpy library learnt from W3Schools. 

# Numpy

- In Python we have lists that serve the purpose of arrays, but they are slow to process.
- NumPy aims to provide an array object that is up to 50x faster than traditional Python lists.
- The array object in NumPy is called `ndarray`, it provides a lot of supporting functions that make working with `ndarray` very easy.
- Arrays are very frequently used in data science, where speed and resources are very important.

# Why is NumPy Faster Than Lists?

- NumPy arrays are stored at one continuous place in memory unlike lists, so processes can access and manipulate them very efficiently.
- This behavior is called locality of reference in computer science.
- This is the main reason why NumPy is faster than lists. Also it is optimized to work with latest CPU architectures.

# Which Language is NumPy written in?

- NumPy is a Python library and is written partially in Python, but most of the parts that require fast computation are written in C or C++.

# Data Types in NumPy

NumPy has some extra data types, and refer to data types with one character, like `i` for integers, `u` for unsigned integers etc.

Below is a list of all data types in NumPy and the characters used to represent them.

- `i` - integer
- `b` - boolean
- `u` - unsigned integer
- `f` - float
- `c` - complex float
- `m` - timedelta
- `M` - datetime
- `O` - object
- `S` - string
- `U` - unicode string
- `V` - fixed chunk of memory for other type ( void )

# The Difference Between Copy and View

- The main difference between a copy and a view of an array is that the copy is a new array, and the view is just a view of the original array.
- The copy *owns* the data and any changes made to the copy will not affect original array, and any changes made to the original array will not affect the copy.
- The view *does not own* the data and any changes made to the view will affect the original array, and any changes made to the original array will affect the view.

# Check if Array Owns its Data

- As mentioned above, copies *owns* the data, and views *does not own* the data, but how can we check this?
- Every NumPy array has the attribute `base` that returns `None` if the array owns the data.
- Otherwise, the `base`  attribute refers to the original object.

# Reshaping arrays

- Reshaping means changing the shape of an array.
- The shape of an array is the number of elements in each dimension.
- By reshaping we can add or remove dimensions or change number of elements in each dimension.

# Iterating Arrays Using nditer()

- The function `nditer()` is a helping function that can be used from very basic to very advanced iterations. It solves some basic issues which we face in iteration, lets go through it with examples.

# Iterating on Each Scalar Element

- In basic `for` loops, iterating through each scalar of an array we need to use *n* `for` loops which can be difficult to write for arrays with very high dimensionality.

# Iterating Array With Different Data Types

- We can use `op_dtypes` argument and pass it the expected datatype to change the datatype of elements while iterating.
- NumPy does not change the data type of the element in-place (where the element is in array) so it needs some other space to perform this action, that extra space is called buffer, and in order to enable it in `nditer()` we pass `flags=['buffered']`.

# Enumerated Iteration Using ndenumerate()

- Enumeration means mentioning sequence number of somethings one by one.
- Sometimes we require corresponding index of the element while iterating, the `ndenumerate()` method can be used for those usecases.

# **Joining NumPy Arrays**

- Joining means putting contents of two or more arrays in a single array.
- In SQL we join tables based on a key, whereas in NumPy we join arrays by axes.
- We pass a sequence of arrays that we want to join to the `concatenate()` function, along with the axis. If axis is not explicitly passed, it is taken as 0.

# Joining Arrays Using Stack Functions

- Stacking is same as concatenation, the only difference is that stacking is done along a new axis.
- We can concatenate two 1-D arrays along the second axis which would result in putting them one over the other, ie. stacking.
- We pass a sequence of arrays that we want to join to the `stack()` method along with the axis. If axis is not explicitly passed it is taken as 0.

# Splitting NumPy Arrays

- Splitting is reverse operation of Joining.
- Joining merges multiple arrays into one and Splitting breaks one array into multiple.
- We use `array_split()` for splitting arrays, we pass it the array we want to split and the number of splits.

# Search Sorted

- There is a method called `searchsorted()` which performs a binary search in the array, and returns the index where the specified value would be inserted to maintain the search order.

# Search From the Right Side

- By default the left most index is returned, but we can give `side='right'` to return the right most index instead.
- **(Too much confusion for these two search sorted ones.)**

# Sorting Arrays

- The NumPy ndarray object has a function called `sort()`, that will sort a specified array.

# Filtering Arrays

- A *boolean index list* is a list of booleans corresponding to indexes in the array.
