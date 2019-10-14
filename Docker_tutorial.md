# History of Virtualization

Earlier, the process for deploying a service was slow and painful. First, the developers were writing code; then the operations team would deploy it on bare metal machines, where they had to look out for library versions, patches, and language compilers for the code to work. If there were some bugs or errors, the process would start all over again, the developers would fix it, and then again the operational team was there to deploy.

There was an improvement with the creation of Hypervisors. Hypervisors have multiple Virtual machines or VMs on the same host, which may be running or turned off. VMs decreased the waiting time for deploying code and bug fixing in a big manner, but the real game changer was Docker containers.

# What is Docker?

Docker is computer software used for Virtualization in order to have multiple Operating systems running on the same host. Unlike Hypervisors which are used for creating VM (Virtual machines), virtualization in Docker is performed on system-level in so-called Docker containers.

As you can see the difference in the image below, Docker containers run on top of the host's Operation system. This helps you to improves efficiency. Moreover, we can run more containers on the same infrastructure than we can run Virtual machines because containers use fewer resources.
![docker_image](/images/docker.png)

Unlike the VMs which can communicate with the hardware of the host (ex: Ethernet adapter to create more virtual adapters) Docker containers run in an isolated environment on top of the host's OS. Even if your host runs Windows OS, you can have Linux images running in containers with the help of Hyper-V, which automatically creates small VM to virtualize the system's base image, in this case, Linux.

# Docker Architecture
Let's talk about Docker main components in the Docker Architecture

* **Docker Engine**

Docker is the client-server type of application which means we have clients who relay to the server. So the Docker daemon called: dockerd is the Docker engine which represents the server. The docker daemon and the clients can be run on the same or remote host, and they communicate through command line client binary, as well as a full RESTful API to interact with the daemon: dockerd.

* **Docker Images**

Docker images are the "source code" for our containers; we use them to build containers. They can have software pre-installed which speeds up deployment. They are portable, and we can use existing images or build our own.

* **Registries**

Docker stores the images we build in registries. There are public and private registries. Docker company has public registry called Docker hub, where you can also store images privately. Docker hub has millions of images, which you can start using now.

* **Docker Containers**

Containers are the organizational units of Docker. When we build an image and start running it; we are running in a container. The container analogy is used because of the portability of the software we have running in our container. We can move it, in other words, "ship" the software, modify, manage, create or get rid of it, destroy it, just as cargo ships can do with real containers.

In simple terms, an image is a template, and a container is a copy of that template. You can have multiple containers (copies) of the same image.

Below we have an image which perfectly represents the interaction between the different components and how Docker container technology works.

![docker container](/images/docker1.png)

For more information on what is docker and how docker works please go through the following **[link!](https://www.guru99.com/docker-tutorial.html)** and also please watch the following **[video](https://www.youtube.com/watch?v=JprTjTViaEA)** for interactive learning.
