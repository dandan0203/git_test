
1,drl�ļ����ڱ���
������ڼ�Ⱥ�У���Ҫ��֤ÿ���ڵ㶼��Ҫ������ļ�
file
2,����hdfs
��ȡ�ļ�
sc.textfileʱ�Ҳ���sc��ͨ��

�����ƶ�ȡ�ļ�ʱ��rule���ز��ˣ�����Ϊbuff��size̫�������¼����˺ܶ�ո�

3,����jar����
��ȡ�ļ�

4.��Ⱥģʽ�£����������˳�������Ϊ�������趨��mater=local[*]


//���غ����ϲ��

stream-processor.properties 
����
phm.fs.defaultFS=hdfs://bigdata1.iline.com:8020
����
#phm.fs.defaultFS=hdfs://phm


#���ز���
#spark.master.url=local[*]
#���ϼ�Ⱥ
spark.master.url=yarn

PHMIoTEventMainStreamController.java
 //        args=new String[2];
 //        //���ϲ���
//        //10.9.1.101
//        args[0]="hdfs://phm";
//        ////args[0]="hdfs://master01.jx.com:8020";
//        args[1]="/phm/stream-processor.properties";

��Ⱥģʽ������ʱ����Ҫ��spark�û���


1.group id��
2.kafka topic���ܴ�������ݣ�


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
>>>>>>> c871092... 第三次版本上�?

<<<<<<< Updated upstream
�����޸�bug
=======
����dev��֧
>>>>>>> Stashed changes
