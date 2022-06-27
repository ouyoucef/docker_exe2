# docker_exe2
cd /home/ubuntu/docker-exe2
docker build -t tomcat:v1 .
docker history 0ebb204b0174
docker inspect  0ebb204b0174
docker run -d --name tomcatcon -p 20200:8080 tomcat:v1
docker ps
docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer -H unix:///var/run/docker.sock
vi /opt/tomcat/conf/tomcat-users.xml
docker image tag tomcat:v1 ouyoucef/tomcat
docker push ouyoucef/tomcat


