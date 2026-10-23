# Download base image of jdk-25 from ghcr.io
FROM ghcr.io/graalvm/jdk-community:25i3

# Create a new deployment workspace
RUN mkdir workspace

# Copy JAR file into deployment workspace
COPY ./tour-management-api-1.0.0.jar /workspace/app.jar

# Allow host to bind port 1403
EXPOSE 1403

# Execute JAR file
ENTRYPOINT ["java","-jar","/workspace/app.jar"]


