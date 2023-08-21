# Create-Post-App


The "Create Posts and Add Comments" project is a microservices-based application built with Node.js, React, Docker, Kubernetes, and Skaffold. The application allows users to create posts and add comments to existing posts. It follows a modular architecture where different services handle specific functionalities.

### Architecture

The project follows a microservices architecture, consisting of the following services:

1. **Client Service**: A React-based frontend that provides a user interface for creating posts and adding comments.

1. **Posts Service**: A Node.js backend service responsible for managing posts. It handles the creation, retrieval, and deletion of posts.

1. **Comments Service**: Another Node.js backend service that manages comments. It handles adding comments to existing posts and retrieving comments for a specific post.

1. **Moderation Service**: A Node.js backend service responsible for moderating comments. It processes comments and applies moderation rules to filter out inappropriate content.

1. **Query Service**: A Node.js backend service that fetches and aggregates data from the Posts Service and Comments Service. It provides a query endpoint to retrieve all posts and their associated comments.

1. **Event Bus**: A service responsible for event handling and communication between the different microservices. It facilitates asynchronous communication and event-driven architecture.

### Technologies Used

The project utilizes the following technologies:

- Node.js: A JavaScript runtime for building the backend services.
- React: A JavaScript library for building the frontend user interface.
- Docker: A containerization platform used for packaging the microservices into containers.
- Kubernetes: An orchestration platform for managing and deploying containerized applications.
- Skaffold: A tool for automating the development workflow, including building, pushing, and deploying containerized applications.

<hr>

### Screenshots
#### The deployed website
![image](https://github.com/MhmoudYahia/Create-Post-App/assets/94763036/60b73810-cb1c-4d56-95e1-75424a8f8fff)
#### The services
![image](https://github.com/MhmoudYahia/Create-Post-App/assets/94763036/ec1b93e1-8a33-496b-80bd-4bcfcc97bf47)

<hr>

### Setup and Installation

To set up and run the project locally, follow these steps:

1. Clone the project repository from \[GitHub URL\].

1. Install Docker on your system to enable containerization.

1. Install Kubernetes and set up a local cluster.

1. Install Skaffold to automate the build and deployment process.

1. Build the Docker images for each microservice using Skaffold.

1. Deploy the microservices to the Kubernetes cluster using Skaffold.

1. Access the client service through the provided URL or port, and start creating posts and adding comments.

### Usage and Examples

Provide examples and usage instructions for different functionalities:

1. **Creating a Post**: To create a new post, send a POST request to the `/posts` endpoint with the required parameters in the request body. Include authentication credentials if necessary.

1. **Adding a Comment**: To add a comment to a post, send a POST request to the `/posts/{postId}/comments` endpoint. Include the comment details in the request body.

1. **Retrieving Comments**: To retrieve comments for a specific post, send a GET request to the `/posts/{postId}/comments` endpoint.

1. **Moderating a Comment**: To moderate a comment, send a POST request to the `/comments/{commentId}/moderate` endpoint. Include the comment ID and moderation action in the request body.

1. **Querying All Posts**: To retrieve all posts and their associated comments, send a GET request to the `/posts` endpoint of the Query Service.

### Troubleshooting

Include a troubleshooting section with common issues and their solutions, such as database connection errors, authentication problems, or deployment-related issues.

### Conclusion

The "Create Posts and Add Comments" project demonstrates a microservices architecture using Node.js, React, Docker, Kubernetes, and Skaffold. By following the provided setup instructions and API documentation, users can successfully create posts, add comments, moderate comments, and query all posts.

Remember to customize the documentation based on your specific project requirements, including the actual API endpoints, environment variables, and any additional configuration steps needed.
