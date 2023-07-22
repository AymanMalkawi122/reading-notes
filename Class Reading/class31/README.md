# Class 31

## Reading  Questions

### Key components of a Docker container

* Docker Image: A Docker image is a lightweight, standalone, and executable package that contains everything needed to run an application, including code, libraries, dependencies, and environment variables.

* Container: A Docker container is an instance of a Docker image. It isolates the application and its dependencies from the host system, providing consistency across different environments.

* Dockerfile: The Dockerfile is a text file used to define the configuration and instructions to build a Docker image. It specifies the base image, adds necessary dependencies, and sets up the environment.

Docker Engine: The Docker Engine is the core of the Docker platform, responsible for creating, running, and managing containers.

### Advantages of Docker containers

* Portability: Docker containers can run on any platform that supports Docker, making it easy to move applications between development, testing, and production environments.
* Isolation: Containers provide isolated environments, reducing conflicts between applications and dependencies.
* Consistency: Docker ensures consistent development and deployment, minimizing the "it works on my machine" problem.
* Scalability: Docker's lightweight architecture allows for easy scaling of applications by running multiple instances of the same container.

### 2. Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates

* Models: Define Django models to represent entities like books, authors, and categories, specifying their fields and relationships.
* Views: Create views to handle HTTP requests and interact with the models to fetch data and render appropriate templates.
* Templates: Design HTML templates to present the data to users, using Django's template language to dynamically insert data.
* URLs: Configure URL patterns in urls.py, linking specific URLs to corresponding views.
* Static files: Serve static files like CSS, JavaScript, and images to enhance the website's appearance.
* Database: Set up a database, such as SQLite or PostgreSQL, to store and manage library data.

### 3. Can you explain the primary differences between Django and Django REST framework?

* Django is a high-level web framework used for building web applications, including complex websites and APIs. It provides features like ORM, forms, admin interface, and URL routing for web development.

* Django REST framework, on the other hand, is an extension of Django that specifically focuses on building RESTful APIs. It simplifies API development by providing tools to serialize Django model data into JSON or other formats and handling common API tasks like authentication, pagination, and permissions.