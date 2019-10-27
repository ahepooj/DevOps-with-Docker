FROM ubuntu:16.04
COPY . .
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs && npm install
CMD ["npm", "start"]
