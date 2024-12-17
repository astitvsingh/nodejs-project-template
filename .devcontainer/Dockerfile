# Use Ubuntu 22.04 LTS as the base image
FROM ubuntu:22.04

# Set non-interactive mode for apt-get to avoid prompts
ENV DEBIAN_FRONTEND=noninteractive

# Set the working directory inside the container
WORKDIR /workspace

# Update the OS packages to their latest versions
RUN apt-get update && apt-get upgrade -y && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Set the default command to keep the container running
CMD ["sleep", "infinity"]
