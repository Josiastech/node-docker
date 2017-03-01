# node-docker

###Bundling and Running the Docker Container

##### Clone the repository and install the dependencies

```bash
$ git clone https://github.com/josiastech/node-docker
$ npm install
```

##### Run the test to make sure averything is working as expected

```bash
$ npm test
```

##### Build the container:
Assuming you alreade have docker installed and can run docker containers in you machine

```bash
$ cd <your project directory>
$ docker build -t node-docker .
#          ^    ^                                      ^
#        build  w/ tag                          this directory

# ... lots of output
```

##### Run the container:

```bash
$ docker run -p 4500:4500 node-docker
#               ^^^^^^^^^
#          bind the exposed container port to host port (on the virtual machine)

```




This is the full implementation for 'Dockerizing a Node.js Web Application' [Check Source].

[Check Source]: https://semaphoreci.com/community/tutorials/dockerizing-a-node-js-web-application