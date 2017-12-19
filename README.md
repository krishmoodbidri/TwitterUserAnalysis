# TwitterUserAnalysis

Analyzing Twitter Dataset (https://snap.stanford.edu/data/twitter-2010.html) on Hadoop to find patterns and analyze the follower patterns between users.

To run :

git clone https://github.com/pahaz/twitter-hadoop-example.git
cd twitter-hadoop-example

mvn compile
mvn package

hadoop jar target/hhd-1.0-SNAPSHOT.jar TwitterFollowerCounter /user/krish94/twitter-2010.txt /user/krish94/count
hadoop jar target/hhd-1.0-SNAPSHOT.jar TwitterAvgFollowers /user/krish94/count /user/krish94/avg
hadoop jar target/hhd-1.0-SNAPSHOT.jar TwitterTopFollowers /user/krish94/count /user/krish94/top
hadoop jar target/hhd-1.0-SNAPSHOT.jar TwitterFollowerCounterGroupByRanges /user/krish94/count /user/krish94/range
