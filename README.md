# Installation of softwares with respect to amazon linux 
<h1>Installation of jdk 8</h1>

 wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u141-b15/336fa29ff2bb4ef291e347e091f7f4a7/jdk-8u141-linux-x64.rpm

 sudo yum install -y jdk-8u141-linux-x64.rpm 

config java if you have multiple java installed

 sudo update-alternatives --config java
<h1> Maven</h1>
 sudo wget https://repos.fedorapeople.org/repos/dchen/apache-maven/epel-apache-maven.repo -O /etc/yum.repos.d/epel-apache-maven.repo 

sudo sed -i s/\$releasever/6/g /etc/yum.repos.d/epel-apache-maven.repo


sudo yum install -y apache-maven

<h1>install epel </h1>

https://www.cyberciti.biz/faq/installing-rhel-epel-repo-on-centos-redhat-7-x/

wget https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm

sudo yum install epel-release-latest-7.noarch.rpm

<h1>Ansible</h1>
after installing epel


sudo yum update

sudo yum install ansible
