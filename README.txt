The Men's running data set 

All the data is taken from http://www.alltime-athletics.com/men.htm
a website by Peter Larsson.
Women data can be obtained here: http://www.alltime-athletics.com/

This repository contains .txt files for the following events:
Men's 100m
Men's 200m
Men's 400m
Men's 800m
Men's 1500m
Men's 5000m
Men's 10000m
Men's Marathon

The .txt files contain in each row an entry similar to this example:
        1      9.58       +0.9    Usain Bolt                     JAM     21.08.86    1      Berlin                        16.08.2009
which encodes information like the position in the list (first entry) the time (second) the name (here fourth) and others.
Each file contains multiple thousand lines of results, i.e. the first thousand best performances in their sports. 
Therefore, it is really the LIST OF BEST PERFORMANCES, NOT WORLD RECORDS.

The raw data has been edited and it is entirely possible that mistakes have been made.
Things that have been changed to handle the date in a better way:
	1) Inserting comma between columns to make it more csv like
	2) For the 100m/200m event, the windspeed was written (in some rows) as +-0 which I transformed to +0 
	3) It was easiert to read times like 01:41.0 than 1:41.0. Therefore I inserted leading zeros in these cases.
	4) Some running results had annotation like 10.01A or 10.01+. I removed these .
