# How to run

Suppose you've already cloned the repository.

You just need:

```
$ make
$ ./HeavyMatcher (-d dataset -m memory -k k)
```

**optional** arguments:

- -d: set the path of dataset to run, default dataset is CAIDA.dat
- -m: set the memory size (KB), default memory is 50
- -k: set the number of top flows, default **k** is 1000

# Output format

Our program will print the Throughput of insertion, AAE, ARE and Precision of these algorithms on the screen.

# TIP 1:  
If there is not enough memory in the running environment, the process may be killed， You can try:
```
 ./HeavyMatcher_simple
```
It runs only the HeavyMatcher and simplifies the process of data preparation.


# TIP 2:
If you need to run the Zipf dataset, you need to change the value of KEY_LEN in params.h to 4 (not 13), because zipf datasets have a different format from other real-world datasets
