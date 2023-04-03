### The evaluation of the performance of the network technologies.
* We would connect the traffic lights esp32 together using the LoRa protocol to exchange informations about the current traffic situtation.
  
### The evaluation of the performance of the embedded devices in terms of power consumption and energy efficiency.
* Each of the esp32s will analize their own camera feed, consuming about 180mA@5V; the only additional power will be of about 20mA required to send and received data from the other esp32s when deciding how to handle the current traffic state.

### The evaluation of the response time from an end-user point of view.
* The response time is very important since it's representative of the efficency of the system, the system should correctly detect veichle and pedestrian and act fast to change the traffic light to adapt the traffic flow.
* The performance of the system could also be evaluated with the number of accident, pollutants in the air and time spent on the junction 
