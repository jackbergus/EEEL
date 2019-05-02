EEEL
====

Do not use the dependencies that you might find in your apt repo. Just use the projects [glog](https://github.com/google/glog) and [gflags](https://github.com/gflags/gflags) as you might find in their most recent GitHub Repo. 

In order to compile the code against these libraries, I made some changes to the Makefile and to the cpp files using the old namespage gflags instead of the most recent google.

-- Giacomo Bergami, 2019
