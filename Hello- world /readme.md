![image](https://github.com/user-attachments/assets/008db4c5-55c2-43db-920b-81fa27c81030)
# Create a freestyle pipeline to print "Hello World!!"
1. Launch your instance in AWS and set up the Jenkins server on your instance using these commands
![image](https://github.com/user-attachments/assets/04cf3329-869a-4e70-8b79-b55dae231080)
````
$ sudo apt-get update
$ sudo apt-get install jenkins
````

```
curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```





Allow inbound traffic on port 8080 for Jenkins in the AWS security group.


Open a new tab and enter your AWS IP address followed by ':8080'. It will prompt you for a password to access your Jenkins server. Use this command to retrieve the password.




After pasting your password, click on 'Install Plugins' to initiate the plugin installation. Create your Jenkins account and the Jenkins dashboard will open.


Follow these steps to create a freestyle pipeline that prints 'Hello World!!'.

Step 1: Click on a new item, and then you will have a page on which you have to give your name to your job and choose ‘freestyle project’ or any other option according to your need and then click ‘ok’.
![image](https://github.com/user-attachments/assets/def3e288-fe8f-40c3-8270-a04cab521361)
```
sudo apt update
sudo apt install openjdk-17-jre
```

Step 2: After this, you will reach a page where you have different options(like build, build triggers, and source code management) that help you manage your job.

Step 3: Now, we will give some description of our job.



Step 4: Now, you have to provide which source code management tool you are using since here we are not using anyone so will choose the ‘none’ option.


Step 5: After this, if you want to give some triggers then you can choose accordingly even Jenkins provides us scheduled triggers. And you can choose to build an environment also accordingly. But, here we are making a simple job, so we are not using any triggers and build environment options.

Step 6: In the build section we have an option ‘Execute shell’ by which we can write some command or code.



echo "Hello friends this is my jenkins demo: %date : %time"


Then click apply and save. So, your job is created.

Step 8: Now, we will run it for which click the ‘build now’ option and a building history will be created then click on it.





