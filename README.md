> ------
>
> > # **Labjack Controller**



## *Description :* 

This package is used to **control [Labjack U3-LV](https://labjack.com/products/u3)** device.
this package contains high level function based on [LabJackPython](https://labjack.com/support/software/examples/ud/labjackpython) package developed by [Labjack](https://labjack.com/) ,this package does not cover all the use cases of the Labjack U3-LV device, it was developed as a layer to manipulate some features(PWM generation, Digital I/O, Analog Input reading,...) and extend the base package with some functionalities (load config from json file, save log to file, ...). 

This package was developed initially for the purpose of commanding a stepper motor for the bending Traction bench

## Dependencies :

To use this package you must install LabjackPython on your environment . To do so copy paste the following command in the command line interface 

`pip install Labjackpython`

