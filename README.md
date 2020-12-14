# HadoopInstallationScripts
Automated installation of Hadoop single-node and multi-node clusters



Instructions for HadoopSingleNode Cluster Setup

1.  Clone the Repository

2.  Within the project directory,exectue the following commands

    2.a.  chmod u+x hadoopSingleNodeInstaller.sh

    2.b.  dos2unix hadoopSingleNodeInstaller.sh

    3.b.  ./hadoopSingleNodeInstaller.sh




Solution:

1) Generate ssh key without password

$ ssh-keygen -t rsa -P ""
2) Copy id_rsa.pub to authorized-keys

$  cat $HOME/.ssh/id_rsa.pub >> $HOME/.ssh/authorized_keys
3) Start ssh localhost

$ ssh localhost
4) now go to the hadoop sbin directory and start hadoop

$./start-all.sh 
./start-all.sh
This script is Deprecated. Instead use start-dfs.sh and start-yarn.sh
Starting namenodes on [localhost]
localhost: starting namenode, logging to /home/amtex/Documents/installed/hadoop/logs/hadoop-amtex-namenode-amtex-desktop.out
localhost: starting datanode, logging to /home/amtex/Documents/installed/hadoop/logs/hadoop-amtex-datanode-amtex-desktop.out
Starting secondary namenodes [0.0.0.0]
0.0.0.0: starting secondarynamenode, logging to /home/amtex/Documents/installed/hadoop/logs/hadoop-amtex-secondarynamenode-amtex-desktop.out
starting yarn daemons
starting resourcemanager, logging to /home/amtex/Documents/installed/hadoop/logs/yarn-amtex-resourcemanager-amtex-desktop.out
localhost: starting nodemanager, logging to /home/amtex/Documents/installed/hadoop/logs/yarn-amtex-nodemanager-amtex-desktop.out
5)password not asking

$ jps 
12373 Jps
11823 SecondaryNameNode
11643 DataNode
12278 NodeManager
11974 ResourceManager
11499 NameNode
