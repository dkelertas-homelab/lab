FROM ubuntu:24.04
RUN apt-get update && apt-get install -y curl
RUN mkdir -p /app/data
RUN curl -o /app/file.txt https://example.com/file.txt
WORKDIR /app
COPY greet .
CMD ["./greet"]
