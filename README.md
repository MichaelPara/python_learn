# python_learn
This project records how I start to learn python programming


# **setup environment**
	+ install vagrant
          open DOS  and input 
          > vagrant box add bento/ubuntu-16.04
          > vagrant box list
          > mkdir c:\test
          > cd c:\test
          > cp c:\User\xulin\github.rsa . 
          > vagrant init bento/ubuntu-16.04
          > vagrant up
        + setup vm
          use putty to login vm
          > cp /vagrant/github.rsa /home/vagrant/.ssh/
          > chmod 700 ~/.ssh/github.rsa
          >  eval $(ssh-agent -s)
          >  ssh-add /home/vagrant/.ssh/github.rsa
        + creat a new repository named python_learn on github
        + clone/modify proj
          > git clone git@github.com:MichaelPara/python_learn.git
          > cd python_learn
          > git branch test
          > git checkout test
          > vim README.md
          > git add .
          > git commit  -m "First change"
          > git checkout master
          > git merge test
          > git push origin master

        + setup python 
          > python3 --version   3.5.2
  
        + setup golang
          > sudo apt-get update 
          > sudo apt-get install golang-go
          > go version   1.6.2

        + gcc/g++ 
          > gcc -v            5.4.0
          > ldd --version     glibc 2.23

        + setup java
          > sudo apt-get install openjdk-8-jdk
          > java -version
          > sudo apt-get install maven
       
         set JAVA_HOME
          > sudo update-alternatives --config java
           add JAVA_HOME="/usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java"
           to /etc/environment
          > sudo vim /etc/environment
          > source /etc/environment
          > echo $JAVA_HOME






