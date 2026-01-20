# Simple DevOps Pipeline

This is a simple Python web application built with Flask that displays a "Hello Build Trigger." message. This project is part of a Google Cloud Platform (GCP) lab focused on building a DevOps pipeline.

The project demonstrates a simple CI/CD pipeline that can be set up to detect changes in a repository, trigger a build, create a Docker image, and upload it to an artifact repository.

![Pipeline Workflow](./workflow.png)

## Project Structure

```
.
├── Dockerfile
├── main.py
├── requirements.txt
├── templates
│   ├── index.html
│   └── layout.html
└── workflow.png
```

## Getting Started

There are two ways to run this application: locally using Python or with Docker.

### Running Locally

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/manasyesuarthana/simple-devops-pipeline
    cd simple-devops-pipeline/
    ```

2.  **Create and activate a virtual environment:**

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the application:**

    ```bash
    python main.py
    ```

    The application will be running at `http://localhost:8080`.

### Running with Docker

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/manasyesuarthana/simple-devops-pipeline
    cd simple-devops-pipeline/
    ```

2.  **Build the Docker image:**

    ```bash
    docker build -t simple-devops-pipeline .
    ```

3.  **Run the Docker container:**

    ```bash
    docker run -p 8080:80 simple-devops-pipeline
    ```

    The application will be running at `http://localhost:8080`.

## GCP Lab

This project is a part of a GCP (Google Cloud Platform) lab: [Building a DevOps Pipeline](https://www.skills.google/paths/20/course_templates/41/labs/613369)

The tasks that have been completed are the following:

*   Create a simple Python application
*   Test the web application in Cloud Shell
*   Define a Docker build using a Dockerfile
*   Manage Docker images with Cloud Build and Artifact Registry
*   Automate builds with triggers
*   Test build changes
