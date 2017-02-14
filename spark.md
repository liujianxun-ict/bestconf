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
We use [HiBench](https://github.com/intel-hadoop/HiBench) that is a widely adopted benchmark tools in the workload generator for Spark to generate the target workload. Currently, the workload adopted in our test is Pagerank. Figure 1 plot the highly differed performance surfaces for Spark Pagerank workload.
<table border="0" cellspacing="0" cellpadding="0" frame=void rows=none cols=none rules=none>
<tr border="0">
<td border="0">
<img src="https://github.com/liujianxun-ict/bestconf/blob/master/pics/spark-pagerank.jpg" width = "800" height = "500" align=center />
</td>
</tr>
<tr border="0">
<td border="0" align=center>
Figure 1: The performance surface of Spark under Hibench-Pagerank workload
</td>
</tr>
</table>
Best Configuration for Spark
--------
We tuned 31 parameters for spark, the best value for each parameter is shown in spark-defaults.conf and spark-env.sh.
Script files
--------
[Scripts for Master node]
[Scripts for Slave node]
Interface Impl
-------
The source files of SparkConfigReadin.java and SparkConfigWrite.java implement the interfaces of ConfigReadin.java and ConfigWrite.java respectively.  




