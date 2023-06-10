
# Class 16

## Reading  Questions

### 1. What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

* No Server Management: Developers are relieved from server provisioning, scaling, and infrastructure management.

* Event-driven Execution: Serverless functions are triggered by specific events or requests, and the infrastructure automatically scales based on demand.

* Pay-per-Use Billing: Billing is based on actual execution time, providing cost optimization.

* Stateless Execution: Functions are stateless, enabling easy scaling and parallel execution.

* Automatic Scalability: Serverless platforms automatically scale functions based on workload, handling sudden spikes in traffic.

* Rapid Deployment and Scaling: Functions can be deployed independently, and the infrastructure manages scaling and distribution.

### 2. How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

1. Create an account on Vercel's website.
2. Install the Vercel CLI (Command Line Interface) tool on your local machine.
3. Set up your project using the Vercel CLI by logging in and initializing your project.
4. Create a serverless function in your project, which will handle incoming requests.
5. Deploy your project using the Vercel CLI and follow the prompts.
6. Test and monitor your deployed serverless function using the provided URL.
7. Customize your deployment with options like custom domains, environment variables, and routing.
8. Scale your serverless functions easily to handle increased traffic or load.

### 3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

APIs, or Application Programming Interfaces, enable software applications to communicate with each other.

***To use APIs in Python applications:***

1. Explore the API documentation to understand available endpoints and request parameters.
2. Make API requests using libraries like ***requests***, specifying the URL, method, headers, and parameters.
3. Handle the API response, accessing and manipulating the data as needed.
4. Process and manipulate the retrieved data according to the application's requirements.
5. Implement error handling to address potential issues during API interactions.
6. Integrate the retrieved data into the Python application for display, analysis, or other purposes.

### 4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?

The Requests library is a popular Python library used for making HTTP requests. It provides a high-level interface and simplifies the process of interacting with APIs by handling the underlying complexities of sending and receiving HTTP requests.

### ***Example***

```python
import requests

# Send a GET request to an API endpoint
response = requests.get('https://api.com')

# Check the response status code
if response.status_code == 200:
    # The request was successful
    data = response.json()  # Get the response data in JSON format
    # Process the data as needed
    for post in data:
        print(post['title'])
else:
    # The request was not successful
    print('Error:', response.status_code)
```

## Things I want to know more about

process communication using sockets
