# Use a lightweight base image
FROM alpine:latest

# Set the working directory
WORKDIR /app

# Copy HTML and CSS files into the container
COPY index.html .
COPY styles.css .

# Install Python (for a simple HTTP server)
RUN apk add --no-cache python3

# Expose port 9001
EXPOSE 9001

# Start a simple HTTP server to serve the files

CMD ["python3", "-m", "http.server", "9001"]