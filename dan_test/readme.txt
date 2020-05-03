
1,drl文件放在本地
如果是在集群中，需要保证每个节点都需要有这个文件
file
2,放在hdfs
读取文件
sc.textfile时找不到sc，通过

二进制读取文件时，rule加载不了，是因为buff的size太长，导致加载了很多空格

3,放在jar包中
读取文件

4.集群模式下，程序总是退出，是因为程序中设定了mater=local[*]


//本地和线上差别：

stream-processor.properties 
本地
phm.fs.defaultFS=hdfs://bigdata1.iline.com:8020
线上
#phm.fs.defaultFS=hdfs://phm


#本地测试
#spark.master.url=local[*]
#线上集群
spark.master.url=yarn

PHMIoTEventMainStreamController.java
 //        args=new String[2];
 //        //线上测试
//        //10.9.1.101
//        args[0]="hdfs://phm";
//        ////args[0]="hdfs://master01.jx.com:8020";
//        args[1]="/phm/stream-processor.properties";

集群模式下运行时，需要用spark用户。


1.group id？
2.kafka topic中能存多少数据？


./kafka-console-consumer.sh --new-consumer --bootstrap-server master01:6667 --topic sequence_device_report --from-beginning
./kafka-console-consumer.sh --new-consumer --bootstrap-server master01:6667 --topic sequence_phm_alarm_report --from-beginning
./kafka-console-consumer.sh --new-consumer --bootstrap-server master01:6667 --topic sequence_phm_alarm_report_fq_test01 --from-beginning
./kafka-console-consumer.sh --new-consumer --bootstrap-server 10.9.1.48:6667,10.9.1.59:6667,10.9.1.99:6667 --topic sequence_device_report_test01 --from-beginning

<<<<<<< HEAD
###############
=======
###############
asohkj
sdfsd
sas
asda
asfsd
>>>>>>> c871092... 绗笁娆＄増鏈笂绾?

<<<<<<< Updated upstream
紧急修复bug
=======
创建dev分支
>>>>>>> Stashed changes
