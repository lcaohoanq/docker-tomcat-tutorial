# docker-tomcat-tutorial
A basic tutorial on running a web app on Tomcat using Docker

See tutorial here - https://www.softwareyoga.com/docker-tomact-tutorial/

# Steps
* Install [Docker](https://docs.docker.com/install/).
* Clone this repository 

```bash
git clone https://github.com/softwareyoga/docker-tomcat-tutorial.git
cd 'docker-tomcat-tutorial'
docker build -t mywebapp .
# docker run -p 80:8080 mywebapp
docker run --ulimit nofile=122880:122880 -p 8081:8080 mywebapp
```

- Access: http://localhost:8081

# Links
[Sample Tomcat web app](https://tomcat.apache.org/tomcat-8.0-doc/appdev/sample/)
