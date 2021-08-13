# debian-container-files
[![Docker Repository on Quay](https://quay.io/repository/prashantdawar/debian-containers/status "Docker Repository on Quay")](https://quay.io/repository/prashantdawar/debian-containers)

Debian Latest ContainerFile
Repo Link: quay.io/prashantdawar/debian-containers:latest





Image Build:

    podman build -t quay/io/prashantdawar/debian-containers:latest -f ContainerFile .





Container Starting:

    podman run -it --name=debian-latest -p 8080:8080 -p 8081:80 -u 0 --rm --entrypoint bash quay.io/prashantdawar/debian-containers:latest