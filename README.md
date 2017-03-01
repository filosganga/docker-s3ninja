# S3 Ninja docker image

# What is S3 Ninja?
S3 ninja emulates the S3 API for development and testing purposes.
For more details visit the [S3 Ninja Homepage](http://s3ninja.net/) and the 
[S3 Ninja GitHub page](https://github.com/scireum/s3ninja)

# How to use this image

Quick run:
```console
$ docker run --rm filosganga/s3ninja
```

To override default AWS credentials:
```console
$ docker run --rm -eAWS_ACCESS_KEY=AKIAIOSFODNN7EXAMPLE -eAWS_SECRET_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY filosganga/s3ninja
```

To mount an external data volume:
```console
$ docker run --rm -v${PWD}/my-data:/s3ninja/data filosganga/s3ninja
```

The image expose the `9444` port and `/s3ninja/data` volume.