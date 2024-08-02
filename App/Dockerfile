# Use the official Tomcat image as the base image
FROM tomcat:10.1

# Set environment variables
ENV POSTGRES_DB=webapplication
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=postgresql

# Copy the WAR file to the webapps directory of Tomcat
COPY target/web-app.war /usr/local/tomcat/webapps/

# Expose port 8080 to be accessible outside the container
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]
