# Required Hardware

This section lists the key hardware required to operate Yonah's ROS Packages

- [Required Hardware](#required-hardware)
- [Common](#common)
  - [RUT955 Cellular Router](#rut955-cellular-router)
  - [SIM Card](#sim-card)
  - [Rockblock 9603](#rockblock-9603)
- [Air](#air)
  - [Beaglebone Black Industrial](#beaglebone-black-industrial)
  - [Cube Black](#cube-black)
  - [Wiz Serial to Ethernet](#wiz-serial-to-ethernet)
  - [Button & Buzzer](#button--buzzer)
- [Ground](#ground)
  - [Laptop](#laptop)
  - [Land/Air Vehicles](#landair-vehicles)

# Common

Hardware that is required on both air and ground sides

## RUT955 Cellular Router

![RUT955](images/ogc/development/sms-link/rut955.png)

Connects the aircraft and the GCS to the Internet and SMS communication through the cellular network. Any cellular router would work, but the code is written specifically for the RUT955. It should be able to work with all Teltonika RUT*** models, but any other models may require tweaks to the code. 

## SIM Card

The SIM card allows us to connect to the internet and cellular networks. Without this the router would be useless. 

## Rockblock 9603

![Rockblock 9603](images/ogc/development/sbd-link/9603.jpeg)

The rockblock connects us to Iridium satellites in order for the SBD node to work. Other satellite devices will work, but some modification of the code may be required. 

# Air

Hardware that is required exclusively on air side

## Beaglebone Black Industrial

![Beaglebone Black Industrial](images/getting-started/required-hardware/BBB.png)

We use a Beaglebone Black Industrial as a companion computer to run all our custom software. It is linked to the router for communication with the ground. It is also the device which stores the mission files which will be needed by the autopilot. 

## Cube Black

![Cube Black](images/getting-started/required-hardware/Cube.png)

The cube is the autopilot responsible for piloting the aircraft. 

## Wiz Serial to Ethernet

![W5500S2E_Z1](images/getting-started/required-hardware/Wiz.jpg)

The WIZ serial to ethernet board is used to physically link the Cube Black to our RUT955 so that data can be transferred between our companion computer and the cube, as well as with the ground control station to afford more command and control to the operators. 

## Button & Buzzer

![Button](images/ogc/development/rff/Button.jpg)![Buzzer](images/ogc/development/rff/Buzzer.jpg)

The button and buzzer are crucial in the safe operation of Nemo. The button is used to let the plane know when it is safe to take off again, and the buzzer is able to warn people around the aircraft to stay clear when it is about to be armed. Any passive button and continuous internal buzzer that can achieve the same objectives can be used. 

# Ground

Hardware that is required exclusively on ground side

## Laptop

A laptop with Ubuntu 20.04 is required to run the Ground Control System to control a fleet of aircraft. 

## Land/Air Vehicles
| type   | name   | fc   | sensor1   | sensor2   |
|:---|:--:|:--:|:--:|---:|
| land   |  jetbot  | jetson nano   |  camera  |    |
|    |    |    |    |    |
| Air   | bebop2   | apm(?)   | android  |  fpv camera  |
|    |    |    | arduino wifi   |    |
|   * | APM   | pixhracer  | gymbol   | fpv camera   |
|    |    | pixhawk mini(?)   | raspi   |    |
|    | dji   | naza m lite   |  fpv camera  |    |
|    |    |    |follding    |  -  |
|    |    |  -  |  -  |  -  |
|    | jti   | pixhawk   | -   | -   |
|    |    |    |  -  |  -  |
|    |  sky (흰색) |  naze32   | camera   |  -  |
|    |    | cleanflight   |  -  | -   |
|    | Darl   | spracing f3 6dot   |    |    |
|    |    |    |    |    |
| RC   | Devention   |  -  |  -  | -   |
|    |    |  devo F12e (black)  |  -  |  -  |
|    |  radiolink  |  -  |   - |  -  |
|    |    |    | -   |  -  |
|    |  shanwan  |  os3  |  for jetbot  |    |
|    |    |    |    |    |
| Module   | LORA Gateway   |  -  |  -  |  -  |
|    | Lora Shield   | -   |  -  | -   |
|    | Arduino mono   |  -  |  -  |  -  |
|    | Arduino wifi   |  -  |  -  |  -  |
|    |  Raspi 4  |    |    |    |
|    |    |    |  -  |  -  |
|    |    |    | -   |  -  |
|  Board  | Jetson nano   |    |  -  |  -  |
|    |    |    |   - |  -  |
|    |  Jetson AGX Xavier  |    |  -  |  -  |
|    |    |    |  -  |   - |
|  Sensors  | Ambient   |  temp  |  humid  |  -  |
|    | 3d camera   |  usb  |  -  |  -  |
|    | IR   | 5cm   |  -  |  -  |
|    |    |    |  -  |   - |
| Parts   | Uart   |  2  | -   | -   |
|    |    |    |  -  |  -  |
|    |    |    |  -  |   - |
|    |    |    | -   |  -  |
