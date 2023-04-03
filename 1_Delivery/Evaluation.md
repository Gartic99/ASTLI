### The evaluation of the performance of the network technologies.
* We would connect the traffic lights esp32 together using the LoRa protocol to exchange informations about the current traffic situtation.
  
### The evaluation of the performance of the embedded devices in terms of power consumption and energy efficiency.
* esp32s camera usage requires about 180mA@5V; 
* WiFi data transfer to the central server to request green light authorization will require 80mA;
* LoRa protocol requires 20mA to send and received data to share environmental data.

### The evaluation of the response time from an end-user point of view.
* The response time is very important since it's representative of the efficency of the system, the system should correctly detect veichle and pedestrian and act fast to change the traffic light to adapt the traffic flow.
* The performance of the system could also be evaluated with the number of accident, pollutants in the air and time spent on the junction 
