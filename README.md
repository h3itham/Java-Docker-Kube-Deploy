# Java-Docker-Kube-Deploy

This repository contains code and resources for deploying Java applications using Docker and Kubernetes. The repository includes sample Java applications, Dockerfiles for building Docker images, and Kubernetes manifests for deploying the applications to a Kubernetes cluster.

The code in this repository is based on the code provided in [h3itham's Java-Docker-Kube-Deploy repository](https://github.com/h3itham/Java-Docker-Kube-Deploy.git).

## Getting Started

To get started with this repository, you'll need to have Docker, Kubernetes, and Maven installed on your local machine or cluster. Once you have those installed, you can clone this repository and start deploying the sample Java applications.

## Building with Maven

To build a Java application with Maven, navigate to the root directory of the application and run the following command
```bash
mvn clean package
```

This will compile the Java code and create a JAR file in the `target` directory.

## Deploying Java Applications

To deploy a Java application using Docker and Kubernetes, follow these steps:

1. Build a Docker image for your Java application using the provided Dockerfile. Run the following command from the root directory of the application
   ```bash
   docker build -t <image-name> .
   ```

   Replace  `<image-name>` with a name for your Docker image.

2. Push the Docker image to a Docker registry. Run the following command
   ```bash
   docker push <image-name>
   ```

3. Create a Kubernetes deployment manifest for your Java application. Use the provided `deployment.yaml` file as a template and replace the `<image-name` placeholder with the name of your Docker image.

4. Apply the deployment manifest to your Kubernetes cluster. Run the following command

   ```bash
   kubectl apply -f deployment.yaml
   ```

   For more detailed instructions on deploying Java applications using Docker and Kubernetes, see the [documentation](https://docs.docker.com/samples/java/) provided by Docker.


## Contact Information

If you have any questions or feedback about this repository, please contact me at [haithamelabd@outlook.com](mailto:haithamelabd@outlook.com).

## Acknowledgments

This repository was inspired by the [Java on Kubernetes](https://github.com/kubernetes/examples/tree/master/java) example provided by Kubernetes.


​    

   

   
