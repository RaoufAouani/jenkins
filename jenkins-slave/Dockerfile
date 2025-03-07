FROM jenkins/jenkins:lts
USER root

# Install Docker
RUN apt-get update && \
    apt-get install -y curl && \
    curl -fsSL https://get.docker.com | sh

# Add Jenkins to Docker group
RUN usermod -aG docker jenkins

USER jenkins
