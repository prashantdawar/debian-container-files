# debian-container-files
[![Docker Repository on Quay](https://quay.io/repository/prashantdawar/debian-containers/status "Docker Repository on Quay")](https://quay.io/repository/prashantdawar/debian-containers)

Debian Latest ContainerFile
Repo Link: quay.io/prashantdawar/debian-containers:buster-httpd

Image Build:
podman build -t quay/io/prashantdawar/debian-containers:buster-httpd -f ContainerFile .


Container Starting:
(as root user) podman run -it --name=buster-httpd -p 8080:8080 -p 8081:80 -u 0 --rm --entrypoint bash quay.io/prashantdawar/debian-containers:buster-httpd
(as non-root user) podman run -it --name=buster-httpd -p 8080:8080 -p 8081:80 -u 10100 --rm --entrypoint bash quay.io/prashantdawar/debian-containers:buster-httpd

On login run : 
"apachectl -k start" to start httpd