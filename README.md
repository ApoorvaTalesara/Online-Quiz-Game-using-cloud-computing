# Online-Quiz-Game-using-cloud-computing
It is web-based system where quiz is taken online i.e., through the internet or intranet using computer system. It can be observed that the information required can be obtained with ease and accuracy in the computerized system. The user with minimum knowledge about
computer can be able to operate the system easily. Quizzes are currently quite popular among educated people as well as in entertainment performances. Although the quiz can be completed manually, it frequently necessitates extensive planning. Quizzes are a popular source of fun and contribute to an individual's knowledge growth. It is cost effective and time effective.

Step 1 : Go to aws.amazon.com then click on create a free account and choose root user.
Step 2 : Go to services and select EC2.
 To create an instance click on launch instance .
Step 3 : Choose an Amazon Machine Image(AMI).
 Choose AMI: Microsoft Windows Server 2022 Base (in Free Tier)
 No change in Instance Details.
 No change is Storage. Assigned storage is sufficient.
 Add a tag: Key: Name
 Value: instance_1 (name of instance you want)
 Security Group Configuration: Add Rules: Custom TCP protocol and set port number to 8080. Add RDP, HTTP and HTTPS rules as well.
When asked for Key Pair, select Create a new Key Pair. Name the Key Pair and
create. A .pem file will be downloaded. Know the location of this file for further
use.
 Launch the instance
 Go to EC2>>Instances and wait for the Instance State to display Running Status Check to display 2/2 checks passed before proceeding.
Step 4 : Create RDP Connect.
 Select the instance you created and click on Connect in top panel.
 Navigate to RDP Client section.
 Click on Download remote desktop file, and a .rdp file will be downloaded.
 In the password section, click on Get Password.
 Here, browse and select the Key Pair file we downloaded in the previous step in .pem format. Click on Decrypt Password. You will be redirected to the previous page and will see the password.
 Open the .rdp file now. Click on Connect in the pop-up. You will be asked to enter a password for the
Administrator user. Copy the Decrypted password from the console and past in the dialogue box and
connect to the RDP client. Click on Yes if another pop-up appears.
 As we have chosen Windows AMI, a VM will open up with Windows OS. Wait till you see the instance details on the Desktop of this VM before moving further. Select Refresh by right-clicking in the VM if you don’t see the details in the top right corner.
 RDP Connection is now established.
To Run the project, you will need to turn off the firewall by going to windows and turning off public and private firewall and go to firewall settings and then go to the advanced settings to allow inbound
connections.
To run this project, install Xampp. You open Apache and MySQL connection on Xampp, create a database by the name of project in phpMyAdmin and import the .sql file.
Step 5 : Import your project in RDP client.
 Open your browser and type : localhost/project_name(localhost/dashboard)
Type on your browser the public IP address displayed on the top right corner of the RDP screen along with the name of the project. (65.0.101.60/dashboard)
 Test the project to see if the database is being saved in phpmyadmin
