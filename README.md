# debian-container-files
[![Docker Repository on Quay](https://quay.io/repository/prashantdawar/debian-containers/status "Docker Repository on Quay")](https://quay.io/repository/prashantdawar/debian-containers)

Debian Buster Apache ContainerFile
Repo Link: quay.io/prashantdawar/debian-containers:buster-httpd
Container Starting:
podman run -it --name=buster-httpd -p 8080:8080 -p 8081:80 -u 0 --rm --entrypoint bash quay.io/prashantdawar/debian-containers:buster-httpd
on login run : "apachectl -k start" to start httpd