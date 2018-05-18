# PyCon mini Osaka 2018 Demonstration

This project includes demonstration code for the presentation at [PyCon mini Osaka 2018](https://osaka.pycon.jp/) at May 19th 2018.

## Prerequisites

* Docker

## Start Jupyter

Build docker image as follows. Don't forget the last `.` (dot). This is required only once.

    docker build -t pyconmini-osaka-2018 .

Then run jupyter notebook like this

    docker run --rm -p 8888:8888 -v $(pwd):/opt/local/work pyconmini-osaka-2018 

To debug docker environment, run bash as follows.

    docker run --rm -ti pyconmini-osaka-2018 /bin/bash -l

# References

* [Jupyter Docker Stacks](https://github.com/jupyter/docker-stacks/)
