# Use Go 1.19 base image
FROM golang:1.19

# Set working directory
WORKDIR /app

# Copy go.mod and go.sum first (to leverage caching)
COPY go.mod go.sum ./
RUN go mod download

# Copy the rest of the backend code
COPY . .

# Expose backend port
EXPOSE 8080

# Run the Go server with environment variables
CMD ["sh", "-c", "go run main.go"]

