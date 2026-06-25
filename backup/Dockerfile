FROM ubuntu:24.04
RUN apt-get update && apt-get install -y curl jq
ENV APP_ENV=production
ENV PORT=8080
ENV LOG_LEVEL=info
EXPOSE 8080
EXPOSE 443
WORKDIR /app
COPY backup .
RUN chmod +x backup
COPY . .
ENTRYPOINT ["./backup"]
CMD ["list"]
