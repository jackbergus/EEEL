EEEL
====

In order to better compile the project, I suggest to first install glog from the apt repos:

     sudo apt-get install -y libgflags-dev

Then, clone the [gflags](https://github.com/gflags/gflags) project and install it. Then, just compile the current project.

In order to compile the code against these libraries, I made some changes to the Makefile and to the cpp files using the old namespage gflags instead of the most recent google.

-- Giacomo Bergami, 2019
