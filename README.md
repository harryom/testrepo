# Multi-Storey Parking Lot System

Automated ticketing system for parking lot that can work without human intervention. It can issue ticket by registration number and vehicle color. If parking space is not available it will show appropriate message for that. When leaving the parking lot parking bill is generated to the customer.

There are two modes for using the system.

1) Interactive command prompt based shell where commands can be typed in.
2) Provide file with instructions and read the commands from that file.

## Getting Started

Follow these instructions to get the project up and running on your local machine for development and testing purposes.

### Prerequisites
Required softwares to be install before using parking lot system.
```
Apache Maven 3.3.9  
JAVA 8
```

### Build

#### How to setup the system and execute test cases
```
cd parking_lot
bin/setup
```
### How to use the system
List of supported commands.
```
create_parking_lot <number of slots>
park <registration number> <color>
leave <slot number>
status
registration_numbers_for_cars_with_colour <color>
slot_numbers_for_cars_with_colour <color>
slot_number_for_registration_number <registration number>
exit
```
#### How to run the system in interactive mode
Execute parking_lot script without any argument. It will start shell for parking lot.
you can use commands from list of supported commands to use the system. 
Enter 'exit' to close the shell.
```
bin/parking_lot
```
Input:

```sh
$ create_parking_lot 6
```

Output:

```sh
Created a parking lot with 6 slots
```

#### How to run the system with input file
Provide file path as argument to execution script.
```
bin/parking_lot file_inputs.txt
```
## How to use interactive mode.

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
