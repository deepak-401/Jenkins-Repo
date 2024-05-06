# Jenkins-Repo
This is a Repo for How to Install Jenkins
<h2>Install Jenkins.</h2>
Pre-Requisites:
Java (JDK)

<h2>Install JDK</h2>
sudo apt update
</br>
sudo apt install openjdk-11-jre

<h2>Check java installed or not</h2>
java -version

<h2>Now, you can proceed with installing Jenkins</h2>

curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
</br>
sudo apt-get install jenkins

<h2>Note:  By default, Jenkins will not be accessible to the external world due to the inbound traffic restriction by AWS. Open port 8080 in the inbound traffic rules as show below.</h2>


<h2>After you login to Jenkins, - Run the command to copy the Jenkins Admin Password - sudo cat /var/lib/jenkins/secrets/initialAdminPassword - Enter the Administrator password</h2>
