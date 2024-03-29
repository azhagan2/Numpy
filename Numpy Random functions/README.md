# Numpy Random

# What is a Random Number?

- Random number does NOT mean a different number every time. Random means something that can not be predicted logically.

# Pseudo Random and True Random.

- Computers work on programs, and programs are definitive set of instructions. So it means there must be some algorithm to generate a random number as well.
- If there is a program to generate random number it can be predicted, thus it is not truly random.
- Random numbers generated through a generation algorithm are called *pseudo random*.
- Can we make truly random numbers?
- Yes. In order to generate a truly random number on our computers we need to get the random data from some outside source. This outside source is generally our keystrokes, mouse movements, data on network etc.

# Random Distribution

- A random distribution is a set of random numbers that follow a certain *probability density function*.

### **Probability Density Function:**

- A function that describes a continuous probability. i.e. probability of all values in an array.

# Random Permutations of elements

- The NumPy Random module provides two methods for this: `shuffle()` and `permutation()`.
- 

# Seaborn module

# Visualize Distributions With Seaborn

- Seaborn is a library that uses Matplotlib underneath to plot graphs. It will be used to visualize random distributions.
- Distplot stands for distribution plot, it takes as input an array and plots a curve corresponding to the distribution of points in the array.

# Normal Distribution

- The Normal Distribution is one of the most important distributions.
- It is also called the Gaussian Distribution after the German mathematician Carl Friedrich Gauss.
- It fits the probability distribution of many events, eg. IQ Scores, Heartbeat etc.
- Use the `random.normal()` method to get a Normal Data Distribution.

# Binomial Distribution

- Binomial Distribution is a *Discrete Distribution*.
- It describes the outcome of binary scenarios, e.g. toss of a coin, it will either be head or tails.

# Difference Between Normal and Binomial Distribution

- The main difference is that normal distribution is continous whereas binomial is discrete, but if there are enough data points it will be quite similar to normal distribution with certain loc and scale.

# Poisson Distribution

- Poisson Distribution is a *Discrete Distribution*.
- It estimates how many times an event can happen in a specified time. e.g. If someone eats twice a day what is the probability he will eat thrice?

# Uniform Distribution

- Used to describe probability where every event has equal chances of occuring.
- E.g. Generation of random numbers.

# Logistic Distribution

- Logistic Distribution is used to describe growth.
- Used extensively in machine learning in logistic regression, neural networks etc.

# Multinomial Distribution

- Multinomial distribution is a generalization of binomial distribution.
- It describes outcomes of multi-nomial scenarios unlike binomial where scenarios must be only one of two. e.g. Blood type of a population, dice roll outcome.

# Relation Between Poisson and Exponential Distribution

- Poisson distribution deals with number of occurences of an event in a time period whereas exponential distribution deals with the time between these events.

# Rayleigh Distribution

- Rayleigh distribution is used in signal processing.

# Similarity Between Rayleigh and Chi Square Distribution

- At unit stddev and 2 degrees of freedom rayleigh and chi square represent the same distributions.

# Pareto Distribution

- A distribution following Pareto's law i.e. 80-20 distribution (20% factors cause 80% outcome).

# Zipf Distribution

- Zipf distributions are used to sample data based on zipf's law.
- **Zipf's Law:** In a collection, the nth common term is 1/n times of the most common term. E.g. the 5th most common word in English occurs nearly 1/5 times as often as the most common word.
