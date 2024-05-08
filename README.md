# Your Project Name

| | |
|-|-|
|`Author` | Mirea Nino-Mario

## Description Parking sensor
This Arduino project incorporates an LED that changes color based on the distance detected by an obstacle sensor. The sensor has a detection range of up to 15° within its field of view and can detect obstacles up to 4 meters away.

In the code, each individual distance measurement is transmitted via the serial port for testing purposes. Additionally, when an obstacle is detected within 100 cm (as defined by the constant beep_start), an acoustic signal is activated.

The frequency of the acoustic signals corresponds to the distance from the obstacle. Specifically, the interval between signals (in milliseconds) is determined by multiplying the distance (in centimeters) by 4. For instance, at a distance of one meter, an acoustic signal will be emitted every 400 milliseconds. This interval decreases as the distance shortens, with signals emitted more frequently. When the minimum distance threshold is reached (set to 5 cm in the code as min_distance), the acoustic signal becomes continuous.

Additionally, alongside these auditory cues, an LED visually indicates the distance by changing its color. As the distance decreases, the LED transitions through a spectrum of colors, providing a clear visual representation of proximity to obstacles.

## Motivation

## Architecture

### Block diagram

<!-- Make sure the path to the picture is correct -->
![Block Diagram](schematics/block_diagram.png)

### Schematic

![Schematic](schematics/kicad_schematic.png)

### Components




| Device | Usage | Price |
|--------|--------|-------|
| Activ Buzzer | Buzzer | [1.5 RON](https://www.optimusdigital.ro/ro/audio-buzzere/635-buzzer-activ-de-3-v.html?search_query=buzzer&results=61) |
| Arduino UNO | Microprocesor | [1 RON](https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1119-buton-6x6x6.html?search_query=buton&results=222) |
| Jumper Wires | Connecting components | [7 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html?search_query=set+fire&results=110) |
| Breadboard | Project board | [10 RON](https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/8-breadboard-830-points.html?search_query=breadboard&results=145) |
| Ultrasonic sensor | Sensor |       |
### Libraries

<!-- This is just an example, fill in the table with your actual components -->

| Library | Description | Usage |
|---------|-------------|-------|
| [lib-name1](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |
| [lib-name2](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |

## Log

<!-- write every week your progress here -->

### Week 6 - 12 May

### Week 7 - 19 May

### Week 20 - 26 May


## Reference links

<!-- Fill in with appropriate links and link titles -->

[Tutorial 1](https://www.youtube.com/watch?v=wdgULBpRoXk&t=1s&ab_channel=BenEater)

[Article 1](https://www.explainthatstuff.com/induction-motors.html)

[Link title](https://projecthub.arduino.cc/)
