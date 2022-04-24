# MongoDB Connector for Apache Kafka tutorial shell

This image contains the following:
- Ubuntu OS
- Python 3
- MongoDB Python Driver (PyMongo)
- Kafkacat
- JQ

If you already have Python and the MongoDB shell available on your local machine you do not have to use this image for the MongoDB Kafka tutorials.  It is provided as a convience for those who do you have these tools installed locally.

To build the image:
```docker build -t tutorialshell:0.1 . ```

Once built, simply run the container and launch an interactive shell session:
```docker run -it --rm tutorialshell:0.1 bash```

Note: remember to include the --network if your Kafka or MongoDB is located in a seperate docker network.  For more information see the MongoDB Online documentation.

There is a docker image of [MongoKafkaTutorial](https://hub.docker.com/repository/docker/robwma/mongokafkatutorial) available to use on Docker Hub.
