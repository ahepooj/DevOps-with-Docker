FROM ubuntu:16.04
WORKDIR /app
COPY /backend-example-docker /app
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs && npm install
ENV FRONT_URL=http://localhost:5000
EXPOSE 8000
CMD ["npm", "start"]
