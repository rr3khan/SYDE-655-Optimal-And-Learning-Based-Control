# Adapted from https://medium.com/@18bhavyasharma/setting-up-and-running-jupyter-notebook-in-a-docker-container-d2acd713ce66
# Use an official Python runtime as a parent image
FROM python:3.11

# Install Jupyter Notebook
RUN pip install jupyter
# Install Jupyter gymnasium
RUN pip install gymnasium

# Make port 8888 available to the world outside this container
EXPOSE 8888

# Define environment variable
ENV NAME World

# Run Jupyter Notebook when the container launches
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]