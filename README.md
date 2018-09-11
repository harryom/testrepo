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
## Assumptions
1. Command to set level for parking lot is not defined. current implementation assumes 1 level in parking lot.
Logic is implemented to handle multi-storey implementation. If command for level is defined in future, just need to provide level data to ParkingLotImpl.setLevel();
2. New line is printed after every output.
3. 'status' command prints headers only when there are no cars in the parking lot.
```
Slot No.  Registration No Colour
```
4. 'status' command uses tab space to separate slot no, registration no and colour
5. Command validation is done, in case of invalid command system will ignore invalid command.
