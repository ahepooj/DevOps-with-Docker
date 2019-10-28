FROM python:3.8.0
COPY . .
RUN apt-get update && apt-get install python-pip -y
# Packages are installed one at a time for dependencies
RUN pip install numpy
RUN pip install pandas
ENTRYPOINT ["python"]