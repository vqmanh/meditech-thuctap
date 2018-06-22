# Script install ELK Server

This is script to install ELK server. Please nopte that this script is only work for CentOS 7.

Firstly, please download script and two files config for logstash

If you do not have wget. Please run the following command to install it:

`yum install wget -y`

After that, download three files by following commands:

wget https://raw.githubusercontent.com/thaonguyenvan/meditech-thuctap/master/ThaoNV/ghi-chep-elk/script/ELK-server.sh

wget https://raw.githubusercontent.com/thaonguyenvan/meditech-thuctap/master/ThaoNV/ghi-chep-elk/script/02-openstack.conf

wget https://raw.githubusercontent.com/thaonguyenvan/meditech-thuctap/master/ThaoNV/ghi-chep-elk/script/03-syslog.conf

Run the following command to run the script.

`bash ELK-server.sh`

There are some options for you in this script. Firstly, script will ask you to know whether you want to keep using `firewalld` or not.

<img src="https://i.imgur.com/MP6nrJL.png">

If you want to use firewalld, press `1` and `Enter`

If you do not want to use firewalld, press any button and `Enter`

This script is use to build ELK server to get log of OpenStack system or linux syslog. The script will ask you to get your selection.

<img src="https://i.imgur.com/TkeOz4d.png">

If you want to config this ELK server to get log from OpenStack system, press `1` and `Enter`.

If you want to config this ELK server to get log from linux syslog, press any button and `Enter`.

The script will start automatically.

<img src="https://i.imgur.com/AonudeD.png">

After installed, you can access your dashboard of Kibana by address `http://your-elk-server:5601`

Thanks for using this script,

ThaoNV