# Technology

## Core: Four main parts
- Smart Camera
- Local Area Station
- Pressure sensors
- Web Dashboard

### Semaphore behaviour
Each smart camera will analyze the current traffic situation and will decide if there is the need to ask to turn green its semaphore, in that case a request message will be delivered to the other sensors and the proper decision will be taken.

### Pressure sensors
Pressure sensors will be placed close to each semaphore, and other two sensors with increasing distance: their purpose is to improve camera detection algorithm during night and adverse conditions and detect vehicles queue status.

### Smart Camera
It is the main component of our project: its main purpose is to detect the presence of a traffic jam and adjust the traffic lights to reduce it; they work together with  pressure sensors.

They are used for the detections **a camera with and integrated ESP-32** to capture the images and analize them, and **pollution sensor** that detects the current salubrity of the air, a **microphone** that allows to detect the presence of an emergency vehicle and a **voltage sensor** that allows us to detect the status of the semaphore. Cameras will be connected using LoRa in a ring topology. The data between the cameras will be exchanged via LoRa. The sensors are controlled by a ESP-32 board.

### Local Area Station
Each esp32 collects the data form the releated semaphore of the cross: it elaborates the data and sends the request to turn green its semaphore. Every semaphore has an unique id for identification. 

### Web Dashboard
It is composed by the esp32 server: it displays the current status of the semaphore and allows to tweak the parameters of the algorithm that controls it; it displays also the local environment data.

## Sensors

### Camera with ESP32
<img src="https://github.com/Gartic99/ASTLI/blob/main/img/camera_esp32.jpg" width="400">

### Air Quality Sensor
<img src="https://github.com/Gartic99/ASTLI/blob/main/img/air_sensor.jpg" width="400">

### Microphone
<img src="https://github.com/Gartic99/ASTLI/blob/main/img/microphone.jpg" width="400">

### Current Sensor

<img src="https://github.com/Gartic99/ASTLI/blob/main/img/current-sensor.jpg"  width="400">

## Pressure sensor

<img src="https://github.com/Gartic99/ASTLI/blob/main/img/pressure.jpg" width="400">

## Actuators

### Relay Module

<img src="https://github.com/Gartic99/ASTLI/blob/main/img/relay_module.jpg" width="400">


## Communication
- **esp32s** LoRA: each esp32 will send/receive informations to/from other traffic lights devices.