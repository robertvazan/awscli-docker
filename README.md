# AWS CLI

This is the latest AWS CLI published by Amazon running on base Ubuntu image.
This image is rebuilt daily with latest updates.
It takes awscli from Python Package Index.
Ubuntu image is taken from robertvazan/ubuntu, which builds daily with latest updates.

There is no prescribed way to use this image.
It just contains prepackaged binaries for faster server deploy.
You are expected to write your own Dockerfile around this image.
The only preconfigured thing is `aws` entrypoint, which means parameters can be passed from command line.
File I/O would likely involve exporting volumes in your Dockerfile.

Docker Hub: https://hub.docker.com/r/robertvazan/awscli/

GitHub: https://github.com/robertvazan/awscli-docker
