FROM jenkins/jenkins:lts

# Switch to root user and install docker
USER root
RUN curl -sSL https://get.docker.com/ | sh

# Copy plugins list
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt

# Run the install-plugins script to install the plugins
RUN jenkins-plugin-cli --plugin-file /usr/share/jenkins/ref/plugins.txt
