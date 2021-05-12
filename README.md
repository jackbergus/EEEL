EEEL
====

In order to better compile the project, I suggest to first install glog from the apt repos:

     sudo apt-get install -y libgflags-dev

Then, clone the [gflags](https://github.com/gflags/gflags) project and install it. Then, just compile the current project.

In order to compile the code against these libraries, I made some changes to the Makefile and to the cpp files using the old namespage gflags instead of the most recent Google library. The  [source code](https://github.com/jackbergus/hierarchy_embedding/) from the paper ''[Hierarchical embedding for DAG reachability queries](https://dl.acm.org/doi/abs/10.1145/3410566.3410583)'' provides a minimal working version of the paper solving an [existing bug](https://github.com/ZhitingHu/EEEL/issues/6). 

-- Giacomo Bergami, 2019-2021
