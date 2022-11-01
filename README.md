### build docker image named 'testapp1_image' using current directory as the root of the build context.
```
docker build . -t testapp1_image
```

### run previously created image 'testapp1_image' as 'testapp1' container, bind port 80 of the container to 80 port of the host machine, with memory and cpu limitations.
```
docker run -p 80:80 -d --name=testapp1 --memory="20m" --cpus=1.5 testapp1_image
```