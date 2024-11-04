# Jenkins-Projects
Leveraging Jenkins for CI/CD to roll out multiple applications alongside other similar DevOps tools.

## What is Jenkins CI/CD tool ?
  - Jenkins is a self-contained, open-source automation server that can be used to automate tasks related
to software delivery, testing, and building. It's a DevOps tool that's used to implement continuous
integration/continuous delivery and deployment (CI/CD) workflows.

- First install a java jdk

      sudo apt-get openjdk-21-jdk -y
    
- Install jenkins on ubuntu machine...To use this repository, first add the key to your system

      sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
      https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
    
- Then add a Jenkins apt repository entry

      sudo apt-get install jenkins

- Start Jenkins
You can enable the Jenkins service to start at boot with the command

      sudo systemctl enable jenkins
      sudo systemctl start jenkins
      sudo systemctl status jenkins


    

