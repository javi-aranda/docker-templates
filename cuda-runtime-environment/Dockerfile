FROM nvidia/cuda:12.2.2-cudnn8-runtime-ubuntu20.04

# Install system dependencies
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    wget \
    ca-certificates \
    python3 \
    python3-pip \
    python3-venv \
    python3-dev \
    cuda-toolkit \
    nvidia-gds

# Set up a working directory
WORKDIR /workspace

# Install Jupyter Notebook and other Python dependencies
RUN pip3 install notebook

# Start Jupyter Notebook on container startup
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
