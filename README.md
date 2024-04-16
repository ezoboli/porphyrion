# porphyrion
Roboticizing the warhammer 40k Porphyrion model

The scope of this project is to turn a Warhammer 40k Imperial Knight model into an actual moving model.

The project will have two agents:
- Throne Mechanicum: package residing inside the model that will control servos and communicate through Bluetooth with the Machine Spirit.
- Machine Spirit: mobile phone app that allows the user to connect to the Throne and control the model.

The Throne Mechanicum package has the following components:
- Adafruit ItsyBitsy nRF52840 Express
- Servo Driver Board PCA9685
- SG 9 servos with the following functions:
  - Torso rotation
  - Right arm rotation
  - Left arm rotation
  - Rocket Pod opening/closing

The Throne Mechanicum's power supply is a regular 9 V battery connected directly to the Servo Driver Board.
The Throne Mechanicum's code shall be written in Arduino, since it's good practice for C and it has more documentation
available compared to CircuitPy.

The Machine Spirit will be an Android based app that will send packages to the Throne Mechanicum to 
perform the following functionalities:
- Rotate Torso
- Turn on/off lights
- Turn arms up and down
- Open/Close rocket pod

  At this time I don't know enough about how to write an Android app to perform those operations.

  The Emperor Protects. 
