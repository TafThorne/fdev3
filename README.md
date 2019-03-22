# fdev3
Dockerfile that sets up a basic Go development environment with OpenJFX and a
number of other tools added.

The Docker Image is listed on Docker Hub:
https://hub.docker.com/r/tafthorne/fdev3/

To pull the image:

  docker pull tafthorne/fdev3

An overview of the included libraries is given below.

## Using This Image
The expected way to use this image is to navigate to the working directory
where your source code resides and start an interactive session.

  docker run -ti --volume="${PWD}:/shared" -w "/shared" tafthorne/fdev3

Then within the running container you can call make or gcc as if it were a
native tool.  The libraries added to this image will be in the global include
path.

## GNU GCC

The GNU Compiler Collection is a compiling system that supports several
languages.  This project focuses more on the C and C++ usage.

## spdlog

spdlog is a fast, header only C++ logging library.  For further details please
see their project page.
* https://github.com/gabime/spdlog

## Contributing

Please see the notes in CONTRIBUTING.md.

