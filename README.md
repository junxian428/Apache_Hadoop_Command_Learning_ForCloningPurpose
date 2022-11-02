# Apache_Hadoop_Command_Learning_ForCloningPurpose

CentOS 

total 30gb

/boot 1gb
/swap 3gb
/  25gb

Network I set default 
(Tutorial Video set static ip)



yum install -y epel-release

systemctl stop firewalld

systemctl disable firewalld.service

First and foremost uninstall default JDK by command 

rpm -qa | grep -i java | xargs -n1 rpm -e --nodeps


File

hadoop-3.1.3.tar.gz
jdk-8u212-linux-x64.tar.gz


tar -zxvf hadoop-3.1.3.tar.gz -C /opt/module


Add my_env.sh

source /etc/profile

then command

Java should work

tar -zxvf jdk-8u212-linux-x64.tar.gz -C /opt/module

___________________________________________________________________________________________________________________________________________


![Screenshot (365)](https://user-images.githubusercontent.com/58724748/199487404-05e6d772-b868-4f9e-a6ad-627970d0450f.png)



core-site.xml

<configuration>

   <property>
   
        <name>fs.defaultFS</name>
        
        <value>hdfs://hadoop100:8020</value>
        
   </property>

        <property>
        
                <name>hadoop.tmp.dir</name>
                
                <name>/opt/module/hadoop-3.1.3/data</value>
                
        <property>
        
</configuration>
~
~
~
~


