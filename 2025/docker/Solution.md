ques1->provide a brief explanation of Docker’s purpose in modern DevOps.
Docker is a containerization tool that helps to package applications , its dependencies and its libraries into lightweight , portable containers . These containers are platform independent making them run on any environment ( dev to production) , cloud to physical server. Docker along with CI/CD enables faster deployment, scaling and efficient resource utilization
   
ques2-> Containerization vs virtualization
Virtualization creates VM and allocates underlying OS resources , making them cost inefficient , slower and less portable. requires more infrastructure management and orchestration
Containerization creates containers and uses shared resources as in they only use resources as much as they want , making the containers cost efficient , portable , lightweight and easier to manage. There are tools like kubernetes and CI/CD to manager infra and orchestration.

ques3-> List and briefly describe key Docker terms such as image, container, Dockerfile, volume, and network.
Image:  A standalone,lighweight package that contains the application,its libraries and its dependencies , code , runtime etc. created from docker using build or pulled from dockerhub
Container: A running instance of image
Dockerfile: A set of instructions used to create an image
Volume : A persistent storage mechanism That allows data to survive container restart or be shared between containers 
Network: A bridge that enables communication between 2 containers and external systems 

ques4-> Explain the main Docker components (Docker Engine, Docker Hub, etc.) and how they interact.
Docker engine -> This is the most important component in docker . it runs on host machine allowing to build , run and manage container
Docker daemon-> dockerd is a background service that manages containers
CLI-> command line tool  to interact with docker

CLI (commands) -> Dockerd-> docker engine process -> output screen 

ques5-> the benefits of multi-stage builds and the impact on image size.

Multi-stage builds help create leaner, more efficient Docker images by separating the build process from the runtime environment. This reduces the final image size and enhances security.

ques6-> explain how Docker volumes help with data persistence and why they are useful.
By default, when a Docker container is removed (docker rm), all its data is lost unless it is stored outside the container. Docker volumes provide a way to persist data even if the container is stopped, restarted, or deleted.

ques7-> describe how Docker networking enables container communication and its significance in multi-container applications.

Docker networking allows containers to communicate with each other and external systems while maintaining isolation. It plays a crucial role in multi-container applications, enabling service discovery, security, and performance optimization.




   
