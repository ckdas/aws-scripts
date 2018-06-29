"# aws-scripts" 

aws bootstrap script. Copy paste to Ec2 bootstrap text box

#!/bin/bash
yum update -y
yum install httpd24 -y
service httpd start
chkconfig httpd on
echo "<!DOCTYPE html><html><head><title>Website running</title></head><body>Your website is up and running with Apache/httpd server</body></html>" > /var/www/html/index.html