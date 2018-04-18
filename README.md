# Jumper Virtual Lab Peripheral Model - PCA9539A
This repo contains PCA9539A peripheral to use with [Jumper Virtual Lab](https://vlab.jumper.io).

For more information, visit [the docs](https://docs.jumper.io).

### Prerequisites
- Ubuntu 16.04
- GCC and Make: `apt install build-essential`
- [Jumper Virtual Lab](https://docs.jumper.io)

## Usage
- Fork [this repository](https://github.com/Jumperr-labs/PCA9539A) on GitHub and clone the new repository onto your Linux machine.
- Make sure you have the build prerequisites by running the following:
  
  ```
  bash
  cd /PATH/TO/PCA9539A/REPO
  make
  ```

- If everything worked as expected, you should now have a "_build/PCA9539A.so" file.
- Copy the .so file from the "_build/" directory to your Jumper Virtual Lab working directory (same one as the "board.json" file).
- Add the component to your "board.json" file:

```
json
{
    "name": "PCA9539A",
    "id": 1,
    "type": "Peripheral",
    "file": "PCA9539A.so",
    "config": {
        "pins": {
            "sda": 26,
            "scl": 27,
            "A0": 31,
            "A1": 30,
            "INT": 29,
            "RESET": 28,
            "P00": 11,
            "P01": 12,
            "P02": 13,
            "P03": 14,
            "P04": 15,
            "P05": 16,
            "P06": 17,
            "P07": 18,
            "P10": 19,
            "P11": 20,
            "P12": 21,
            "P13": 22,
            "P14": 23,
            "P15": 24,
            "P16": 25,
            "P17": 3
            }
        }
}
  ```

## License
Licensed under the Apache License, Version 2.0. See the LICENSE file for more information
