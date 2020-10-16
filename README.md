> ------
>
> # **Labjack Controller**



## *Description :* 

This package is used to **control [Labjack U3-LV](https://labjack.com/products/u3)** device.
this package contains high level function based on [LabJackPython](https://labjack.com/support/software/examples/ud/labjackpython) package developed by [Labjack](https://labjack.com/) ,this package does not cover all the use cases of the Labjack U3-LV device, it was developed as a layer to manipulate some features(PWM generation, Digital I/O, Analog Input reading,...) and extend the base package with some functionalities (load config from json file, save log to file, ...). 

This package was developed initially for the purpose of commanding a stepper motor for the bending Traction bench

## *Dependencies :*

To use this package you must install LabjackPython on your environment . To do so copy paste the following command in the command line interface 

```command line 
	pip install Labjackpython
```

## *Package architecture :*

* README.md : Markdown file that contains general description and guidance for the actual project

* LICENSE : This plaintext file describes the license used for this project.

* .gitignore : This is a file that tells Git which kinds of Folders and files to ignore 

* Makefile.py : Python script to make an easy install for the dependencies of the project ( further    explanation on how to use this script will be provided in the following paragraphs)

* Core\ : folder of the source file for this package
     - labjack_controller.py : python module , main script of the package to control a Labjack U3-LV device
     - Helpers.py : python module , contains function that are essential for the main module to work 

* Tests\ : Folder of tests scripts that checks the source files 
     - test_labjack_controller.py : tests suite case for checking the labjack_controller module
     - test_Helpers.py : tests suite case for checking the Helpers

* Data\ : Folder that contains the input and output data of the package

     - Input_Data\ : Folder for the input data

       ​       - Settings. json : Json file for parameters of the labjack module

     - Output_Data\ : Folder for the output data

* Requirements\ : Folder for requirements files 
       -  requirements.dev : File defines outside Python dependencies in development mode
       -  requirements.prod : File defines outside Python dependencies in production mode