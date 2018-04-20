# mbed-js-devi2c
JavaScript wrappers for DevI2C by STMircroelectronics.

# About library
Helper class DevI2C providing functions for multi-register I2C communication common for a series of I2C devices.

# Requirements
This library is to be used with the following tools:
* [Mbed](https://www.mbed.com/en/platform/mbed-os/)
* [JerryScript](https://github.com/jerryscript-project/jerryscript)

See this project for more information: [mbed-js-example](https://github.com/ARMmbed/mbed-js-example)

# Installation
* Before installing this library, make sure you have a working JavaScript on Mbed project.
Follow [mbed-js-example](https://github.com/ARMmbed/mbed-js-example) to create the project.
Make sure the project builds for your target device before proceeding.

* Install this library using npm (Node package manager) with the following command:
```
cd project_path
npm install syed-zeeshan/mbed-js-devi2c
```

# Usage
```
//Initialize DevI2c with SDA and SCL pins
var dev_i2c = DevI2C(sda_pin, scl_pin);

//To use with another library
var hts221 = HTS221_JS();
hts221.init_i2c(dev_i2c);

```

        
# Dependents
This library is requred if using I2C for connecting with the following devices:
* [mbed-js-hts221](https://www.github.com/syed-zeeshan/mbed-js-hts221)
* [mbed-js-lps22hb](https://www.github.com/syed-zeeshan/mbed-js-lps22hb)
* [mbed-js-lsm6dsl](https://www.github.com/syed-zeeshan/mbed-js-lsm6dsl)
* [mbed-js-lsm303agr](https://www.github.com/syed-zeeshan/mbed-js-lsm303agr)
