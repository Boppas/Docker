FROM almalinux
RUN yum install nginx -y
# When image creator is running this below command will not run. When someone Else try to use your image the below image will run
ONBUILD ADD simple.txt /tmp/
