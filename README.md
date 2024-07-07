Description:

This repository provides a Docker Compose setup for seamlessly running an Ollama AI model alongside a Jupyter Notebook environment. This enables you to interact with Ollama models directly within Jupyter Notebooks, leveraging GPU acceleration for enhanced performance.

Features:

Integrated Ollama Service: The ollama service container provides access to the Ollama AI engine, allowing you to call its APIs for model loading, generation, and other functionalities.
Jupyter Notebook Environment: The jupyter service container offers a ready-to-use Jupyter Notebook environment where you can write and execute Python code, experiment with Ollama models, and visualize results.
GPU Acceleration: By leveraging NVIDIA GPUs (if available), the ollama service can process requests faster, especially for computationally intensive models.
Requirements:

Docker: Installation instructions can be found at https://www.docker.com/.
NVIDIA GPU (Optional): If you wish to utilize GPU acceleration, a compatible NVIDIA GPU is recommended.

Getting Started:

1. Clone the Repository:
git clone git@github.com:moh-C/Jupyter-Ollama.git

2. Build and Run the Containers:

Open a terminal or command prompt and navigate to the cloned repository directory.
Run the following command to build and start the Docker containers:

docker-compose up -d
The -d flag runs the containers in detached mode, allowing them to operate in the background.

3. Access Jupyter Notebook:

Open a web browser and navigate to http://localhost:8888.
You might be prompted to enter a password. The default password is root (security note: Consider changing the default password for production use).
