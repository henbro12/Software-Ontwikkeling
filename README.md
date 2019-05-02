# Software Ontwikkeling #
=========================

This project is a simple template that students can use for the assignment of the Software Development course.

## Getting Started ##
---------------------

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites ###

The following tools are required in order to build and run this project:
'''
Atollic TrueStudio for STM32
GIT (e.g. GitHub)
Shippable
'''

### Installing ###

Get repository
'''
Clone this repository to your local folder
'''

Setup tools
'''
Connect your project to GIT and Shippable
'''

Run this project locally
Option 1, Debug:
'''
Use the Debug option to flash the project on the ARM
'''
Option 2, Run:
'''
Install [STSW-LINK004](https://www.st.com/en/development-tools/stsw-link004.html) from STMicroElectronics
* Go to Run > External Tools > External Tools Configurations
* Right-click on Program > New
* Set Location and Working directory to ST-LINK_CLI.exe
* Set arguments to:
	* -c SWD -P ${project_loc}\${config_name:${project_name}}\${project_name}.hex -Rst
* Apply and Exit
* Open Run > Run Configurations...
* Right-click on Launch Group > New
* Add... > choose external tool you've just created for ST-LINK_CLI.exe
* Apply and Exit
The project should now be configured to flash and run it
'''

## Building the project ###
---------------------------

This repository cantains a Makefile which can compile and build the source code.
To use this Makefile, the following commands should be used:
'''
* make       - Displays help dialog
* make clean - Removes all generated files
* make build - Builds the source code
* make all   - Executes 'make clean' and 'make build' respectively
'''

## Running the tests ##
-----------------------

No tests are implemented yet

## Authors ##
-------------

**Henrico Brom** 
Third-year student Electrical Engineering at the Utrecht University of Applied Sciences (02-05-2019)
(Henrico.brom@student.hu.nl)

## Acknowledgements ##
----------------------
* Franc van der Bent (Teacher at Hogeschool Utrecht)
* Michiel Scager (Teacher at Hogeschool Utrecht)
* Jeroen de Bruijn (Graduated student from Hogeschool Utrecht)

