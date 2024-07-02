<b>this is the file of impkementation of calculator</b>
follow this given steps
step 1. Login to  AWS console
step 2. create ec2 machine
step 3. configure security group (select TCP and give sources as 0.0.0.0/0 to allow all traffic )
step 4. connect to ec2 machine on mobaxterm terminal or any through ssh .
step 5. install httpd webserver in machine(used to run web app)
   sudo su
   yum update -y
   yum install httpd -y
   yum install git -y
   cd /var/www/html
   git clone <repository-link>
   cd calculator 
   mv index.html /var/www/html 
   mv script.js /var/www/html
   mv style.css /var/www/html
   mv utils.css /var/www/html
   service httpd start
step 6. access website from browser using ec2 public ip or DNS.
