# Wifi Data extractor for TU Delft

Data-Centric Design - A python application which extracts data from the [Cisco Prime](https://www.cisco.com/c/en/us/products/cloud-systems-management/prime-infrastructure/index.html) infrastructure of TU Delft and streams the data to [Apache Kafka](https://kafka.apache.org/) to be used by researchers. 
The following queries can be fetched by the producers - 
- Client Stats
- Client Sessions
- Client Details
There is a producer program for each query which pushes data to different topics(Daily,Monthly,Vendor) and a consumer program which collects the data and writes it to a csv file.

### Prerequisites

Docker is required to run the system and can be installed by - 

* [Install Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

## Getting Started
You can clone or download the repository to run it on your local machine for development and testing purposes. The docker file will run the environment and also install the necessary libraries like -
* [python package installer](https://pip.pypa.io/en/stable/) 
* [flatten-json](https://pypi.org/project/flatten-json/) 
* [kafka-python](https://github.com/dpkp/kafka-python)
* [Curl](https://curl.haxx.se/)
* [Pandas](https://pypi.org/project/pandas/)

### Installing

The following command builds the images and the containers for the Dockerfile-
```
- docker build .
```
Execute this command to run the dockerfile
```
-  docker-compose up
```
The status of the docker containers can be checked by the following command
```
-  docker ps
```
After this you can run the producer and consumer on different terminals using -

```
- python producer.py
- python consumer.py
```
The consumer will produce the csv fle which can be distributed on authorization levels. 

### Paging for large amount of data

The data can be queried in a [paged](https://solutionpartner.cisco.com/media/prime-infrastructure/api-reference/szier-m8-106.cisco.com/webacs/api/v3/index9df8.html?id=paging-doc) format like -  

- Devices?.full=true&.firstResult=0&.maxResults=4    (First four results(0-3))
- Devices?.full=true&.maxResults=4&.firstResult=4    (four results (4-7))


## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://opensource.org/licenses/MIT) file for details











# Wifi Data

Data-Centric Design

# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- TODO: Access Prime Cisco API
- TODO: Push data into kafka

# Paging via the query string

- Devices?.full=true&.firstResult=0&.maxResults=4    (First four results(0-3))
- Devices?.full=true&.maxResults=4&.firstResult=4    (four results (4-7))

- 
# merge 
- git checkout master
- git pull origin master
- git merge test
- git push origin master
- 


