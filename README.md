# ilinkpilot

1)You can run main class as java progrom from eclipse(IlinkSpringBoot.java) to launch app

2)Command line build
./mvnw clean install dockerfile:build \
-Dorg.springframework.boot.logging.LoggingSystem=org.springframework.boot.logging.log4j2.Log4J2LoggingSystem \
-Dspring.profiles.active=dev


To test it you will put this url on the browser 
http://localhost:8787/dataTime

docker --help 
docker images
docker rmi <images_id>
docker ps


3)docker run -p 8787:8787 -t springio/ilink-spring-boot-docker


4)Openshift commands
  a)oc login -u developer -p developer 
  b)oc new-project ilink 
  c)oc new-app centos/ruby-22-centos7~https://github.com/yrkhanalilink/ilinkpilot 
  d)oc logs -f bc/ilinkpilot 
  e)oc secrets new-basicauth github-credentials --username=<yourgithubusername> --password=<yourgithubpassword>
  
5)Git
git --version

6)SSH
ssh-keygen -t rsa -b 4096
 
 nano ~/.ssh/config
 Host github.com
        IdentityFile ~/.ssh/id_rsa



  
  



