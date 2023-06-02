# Whale-docker
git clone <repository-url>
Replace <repository-url> with the URL of the Git repository you want to clone.

Navigate to the cloned repository: Change your current directory to the cloned repository:

bash
Copy code
cd <repository-directory>
Replace <repository-directory> with the name of the directory created during the cloning process.

Build the Docker image: Use the docker build command to build the Docker image from the Dockerfile. Make sure you have Docker installed on your system. Run the following command:

bash
Copy code
docker build -t myimage .
This command assumes that the Dockerfile is present in the current directory. The -t flag is used to provide a tag (name) for the image. In this example, the tag "myimage" is used, but you can choose any desired name.

Run the Docker container: After the Docker image is built, you can use the docker run command to start a container based on that image and expose it on port 8080. Run the following command:

bash
Copy code
docker run -p 8080:8080 myimage
The -p flag is used to map the container's port to the host's port. In this case, it maps container port 8080 to host port 8080. You can modify the host port number if needed.

Access the application: Once the Docker container is running, you can access the application in your web browser by navigating to http://localhost:8080
