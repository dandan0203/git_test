
1,drlÎÄ¼ş·ÅÔÚ±¾µØ
Èç¹ûÊÇÔÚ¼¯ÈºÖĞ£¬ĞèÒª±£Ö¤Ã¿¸ö½Úµã¶¼ĞèÒªÓĞÕâ¸öÎÄ¼ş
file
2,·ÅÔÚhdfs
¶ÁÈ¡ÎÄ¼ş
sc.textfileÊ±ÕÒ²»µ½sc£¬Í¨¹ı

¶ş½øÖÆ¶ÁÈ¡ÎÄ¼şÊ±£¬rule¼ÓÔØ²»ÁË£¬ÊÇÒòÎªbuffµÄsizeÌ«³¤£¬µ¼ÖÂ¼ÓÔØÁËºÜ¶à¿Õ¸ñ

3,·ÅÔÚjar°üÖĞ
¶ÁÈ¡ÎÄ¼ş

4.¼¯ÈºÄ£Ê½ÏÂ£¬³ÌĞò×ÜÊÇÍË³ö£¬ÊÇÒòÎª³ÌĞòÖĞÉè¶¨ÁËmater=local[*]


//±¾µØºÍÏßÉÏ²î±ğ£º

stream-processor.properties 
±¾µØ
phm.fs.defaultFS=hdfs://bigdata1.iline.com:8020
ÏßÉÏ
#phm.fs.defaultFS=hdfs://phm


#±¾µØ²âÊÔ
#spark.master.url=local[*]
#ÏßÉÏ¼¯Èº
spark.master.url=yarn

PHMIoTEventMainStreamController.java
 //        args=new String[2];
 //        //ÏßÉÏ²âÊÔ
//        //10.9.1.101
//        args[0]="hdfs://phm";
//        ////args[0]="hdfs://master01.jx.com:8020";
//        args[1]="/phm/stream-processor.properties";

¼¯ÈºÄ£Ê½ÏÂÔËĞĞÊ±£¬ĞèÒªÓÃsparkÓÃ»§¡£


1.group id£¿
2.kafka topicÖĞÄÜ´æ¶àÉÙÊı¾İ£¿


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
>>>>>>> c871092... ç¬¬ä¸‰æ¬¡ç‰ˆæœ¬ä¸Šçº¿
