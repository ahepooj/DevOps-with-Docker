FROM ubuntu:16.04
COPY . .
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs && npm install
ENV API_URL=http://localhost:8000
EXPOSE 5000
CMD ["npm", "start"]
