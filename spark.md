BestConf for Spark
======================
Experiment Environment
-----------
We executed Bestconf for the spark cluster with 4 nodes. The spark cluster consists of 1 master node and 3 slave nodes. All nodes used in our experiment are shown below.
<div>
    <table border="0">
      <tr>
        <th>IP address</th>
        <th>Username</th>
        <th>Password</th>
        <th>Type</th>
      </tr>
      <tr>
        <td>172.16.48.41</td>
        <td>root</td>
        <td>ljx123</td>
        <td>Master</td>
      </tr>
      <tr>
        <td>172.16.48.209</td>
        <td>root</td>
        <td>ljx123</td>
        <td>Slave</td>
      </tr>
      <tr>
        <td>172.16.48.211</td>
        <td>root</td>
        <td>ljx123</td>
        <td>Slave</td>
      </tr>
      <tr>
        <td>172.16.48.207</td>
        <td>root</td>
        <td>ljx123</td>
        <td>Slave</td>
      </tr> 
    </table>
</div>

Result
-----------
The benchmark used to test Spark cluster performance is pagerank. Figure 1 plot the highly differed performance surfaces for Spark.
![](https://github.com/liujianxun-ict/bestconf/blob/master/pics/spark-pagerank.jpg)
Figure 1: The performance surface of Spark under Hibench-Pagerank workload.


