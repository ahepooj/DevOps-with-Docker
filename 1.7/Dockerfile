FROM ubuntu:16.04
COPY . .
RUN apt-get update && apt-get install -y curl
RUN chmod +x ./script.sh
CMD bash "./script.sh"