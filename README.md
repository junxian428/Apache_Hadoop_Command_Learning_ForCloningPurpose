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

rpm -ga | grep -i java | xargs -n1 rpm -e --nodeps
