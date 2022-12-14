# Minecraft Docker

This Repo is a Dockerfile with supporting files designed to be a light and fast containerized Minecraft server.  
Running on the java `JDK-17 Oracle` image, the download is quite small and overhead is minimal.

> Java Version: 17

## Reqired

The Dockerfile reqires the following to work properly:

> A `.jar` file that has the latest version of paperMC or Branch  

## How to Compile

Please do the following to compile the docker file:

1. Put the `Dockerfile` along with the *required* files listed above in the same directory (preferably with nothing else)

2. Make sure docker is installed on your system by running  
   ```Dockerfile
   docker version
   ```  
   If you get a version number, docker is installed.  
   If docker is not installed, please install the Docker Engine

3. Once the steps `1` and `2` have been done, run the command  
   ```Dockerfile
   docker build -t <tag> .
   ```  
   > The `<tag>` represents the name you'd like to give your container
   
   > The `Dockerfile` may not compile unless you have a folder name `plugins` in the working Directory.  
   > please see more about it below

## Plugins

In order to add the plugins to the server you must:

1. Create a folder in the same directory of the `Dockerfile` called `plugins`

2. Put all the `.jar` plugin files you'd like in there

3. Compile docker image using instructions above
