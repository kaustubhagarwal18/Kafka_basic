# Wifi Data extractor for TU Delft

A python application which extracts data from the [Cisco Prime](https://www.cisco.com/c/en/us/products/cloud-systems-management/prime-infrastructure/index.html) infrastructure of TU Delft and streams the data to Apache Kafka [Apache Kafka](https://kafka.apache.org/)to be used by researchers.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
- [Install Docker](https://kafka.apache.org/)
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

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

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc










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
- Use multiple consumers in parallel w/ 0.9 kafka brokers# typically you would run each on a different server / process / CPU
- 
# merge 
- git checkout master
- git pull origin master
- git merge test
- git push origin master
- 


