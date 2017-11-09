# Re-constructing the Sum (+) function using Dense networks (classifiers)

Testing out keras functionality by applying it to re-learn how to sum two numbers from 0-99. 
Doing it as a classifier to make the task tougher. 

The input will be two vectors wide representing the numbers being summed up and the target is the sum of the two numbers transformed into a one-hot encoded vector. 
The output of the dense network will 200 classes wide.

Lessons:
 - We need atleast a 1 million records to get a high level of accuracy
 - Normalizing the input vector goes a long way in terms of converging the network fast.
 - The network still doesnt work well on low density classes where we have fewer examples, i.e. when sum is less than 10 or greater than 190 (we have very few numbers that can sum up to these classes). Training more epochs may work or oversampling on minority classes may be required.

