# PySpark-Word-Counter

Here are the brief steps for writing the word counting program:

Created a base RDD from Complete_Shakespeare.txt file.
Used RDD transformation to create a long list of words from each element of the base RDD.
Removed stop words(For example "I", "the", "a" etc., are stop words) from the data.
Created a pair RDD where each element is a pair tuple of ('word', 1)
Grouped the elements of the pair RDD by key (word) and add up their values.
Swapped the keys (word) and values (counts) so that keys is count and value is the word.
Finally, sorted the RDD by descending order and print the 10 most frequent words and their frequencies.
