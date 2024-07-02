<h2><u This is the file of implementation of calculator ></u></h2>
<h3>Follow this given steps</h3>
step 1. Login to  AWS console<br>
step 2. create ec2 instance.<br>
step 3. give configure security group (select TCP and give sources as 0.0.0.0/0 to allow all traffic )<br>
step 4. connect to ec2 machine on mobaxterm terminal or any , through ssh .<br>
step 5. install httpd webserver in machine ( used to run web app )<br>
   sudo su<br>
   yum update -y<br>
   yum install httpd -y<br>
   yum install git -y<br>
   cd /var/www/html<br>
   git clone <repository-link><br>
   cd calculator<br> 
   mv index.html /var/www/html<br>
   mv script.js /var/www/html<br>
   mv style.css /var/www/html<br>
   mv utils.css /var/www/html<br>
   service httpd start<br>
step 6. access website from browser using ec2 public ip or DNS.<br>
