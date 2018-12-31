# mvn package   (use jdk8 to run maven, I found jdk 11 will fail)

# copy the DockerFile and target/spring-boot-crud.jar to docker host

# docker build -t springbootcrud .

# docker image ls

# docker run -p 8080:8080 springcrud

# docker container ls

update the 'VOLUME /tmp' to 'VOLUME /tmp/abcxu', and create the image and exec bash in the container
[root@centostest ~]# docker exec -it 7f4e6fb6c482 ls /tmp
abcxu
hsperfdata_root
tomcat-docbase.3518755318273859916.8080
tomcat.8247241600472789994.8080
