# Challenge 1 - Simple Web Server for Static Web Pages

This project is an introduction to using Docker for serving static web pages. It's a simple setup that uses NGINX to serve an `index.html` file contained within a Docker container.

## Goals

- Learn the basics of Docker.
- Build a Docker image.
- Run the container and view the results in a browser.
- Publish the Dockerfile and related files on GitHub.

## Steps

1. Create a folder named `challenge1` and a subfolder named `public` for static assets.
2. Add an `index.html` file in the `public` folder with your name and student ID.
3. Write a Dockerfile to configure NGINX to serve the content of the `public` folder.
4. Build the Docker image using the provided Dockerfile.
5. Run the Docker container and map the necessary ports.
6. Push the Dockerfile and `public` folder to a GitHub repository.
7. Take a screenshot of the server running and the page being served.
8. Submit the GitHub repository's URL and screenshots on D2L.

## Expected Outcome

When you navigate to `http://localhost:8080/`, you should see a homepage with your name and student ID.

## Instructions for Building and Running the Container

To build the Docker image:

```bash
docker build -t my-static-site .

To run the container: 
docker run --name my-site -d -p 8080:80 my-static-site

Replace my-static-site with your name

After running the container, open your web browser and go to http://localhost:8080 to view your static site.

Author
Aryan Patel
Acknowledgements
Southern Alberta Institute of Technology (SAIT) instructors for their guidance.