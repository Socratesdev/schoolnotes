

| Conventional design                        | Mechatronics design                                |
| ------------------------------------------ | -------------------------------------------------- |
| Bulky                                      | Compact                                            |
| Complex mechanisms                         | Simple mechanisms                                  |
| Cable problems                             | Busor wireless communication                       |
| Connected components                       | Autonomous units                                   |
| Stiff construction                         | Elastic construction                               |
| Analog control                             | Programmable feedback digital control              |
| Non-measurable quantities change arbitrary | control of non-measurable estimated quantities     |
| Simple monitoring                          | supervision with fault diagnosis                   |
| Fixed abilities                            | Leearning abilities                                |
| precision through narrow tolerances        | presision through measurement and feedback control |


*Transducer* is a device that converts one form of energy to another.
*Sensor* detects some characteristics from its environs.
	 Active sensors - requires some form of external power to operate
	 Passive sensors - does not need any additional enery source and directly generates an electrical signal in responce to electrical stimuli.

examples of transducers are:
- Microphones convert sound signals to electrical impulses.
- Solar cell converts light to electricity. 
- Electricl motors convert elecrical to mechanical energy.

The ==output of a sensor== is usually an analog signal. It can be the following types:
- A voltage level with direct correlation to the input.
- A pulse with a modulatated signal.
- A waveform modulated either in amplitude or frequency.


| Analogue signals                                            | Digital singnals                                                       |
| ----------------------------------------------------------- | ---------------------------------------------------------------------- |
| Continuous in both value and time                           | Discontinuous in value and time                                        |
| Can be on, off and an infinite position between 0 and 1     | Has to positions off and on                                            |
| Presented by sime waves                                     | Respresented by square waves                                           |
| Prone to noise during transmission                          | Less prone to noise during transmission                                |
| Low accuracy                                                | Bette accuracy                                                         |
| Analog circuits conpomise fundamental electrical components | Digital corcuits compromise of logic gates and more complex digital IC |
| used in analog devices                                      | Used in digital electronics                                            |


| quantity being measured | input device                                                               |
| ----------------------- | -------------------------------------------------------------------------- |
| Light level             | Light dependant resistor<br>Photodiode<br>Photo-transistor<br>Solar cell   |
| Temprature              | Thermocouple<br>Thermistor<br>Thermostat<br>Resistive temprature detectors |
| Force/Pressure          | Strain gauge<br>Pressure switch<br>Load cells                              |
| Position                | Potentiometer<br>Encoder<br>LVDT                                           |
| Speed                   | Tacho-generator<br>Reflective opto-coupler<br>Doppler effect sensor        |
| Sound                   | Carbon microphone<br>Peizo-electric crystal                                |

| Active sensors                                                                        | Passive sensors                                                                     |
| ------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Requires an exitation signal                                                          | Generates signal without any energy consumption                                     |
| generate electric current or voltage directly in responce to enviromental stimulation | their responce characteristic change according to the change in physical parameters |
| Examples: Thermistor, strain gauge                                                    | Example: Thermocouple, Peizoelectric crystals                                       |

An *actuator* is a mechanism by which an agent works upon an enviroment. It converts enery to motion.

Categories of actuation systems:
- Switching devices: Controls signal switches ON and OFF 
- Electrical devices: A current through a solenoid is used to actuate a soft irom core.
- Electromechanical system: A current is used to drive a motor.
Common forms of acuators are pneumatic, hydraulic,mechanical and elelctrical motors.

###### Pneumatic actuators
It operates on a combination of air and spring force.
###### Hydraulic actuators
Are used for processes requiring quick and accurate responses..

###### Electrical slenoid actuators
These contain a armature and a electrical solenoid. When the solenoid is activated the magnetic force causes the armature to rise up openning the valve and then when the electrical current is turned off the armature falls form the strength of the spring. 
A major advantage of them is their quick operation.


#### Mechanical acuators
They operate by onverting rotary motion to linear motion.
They operate by a simple mechanism such as screw, wheel and axle, cam.
- Screw - by rotating the actuator nut the screw shaft moves in a line.
- Wheel and axle - a rotating wheel moves a cable, rack,or belt to produce linear motion.
- Cam - A wheel like cam rotates and the eccentric shape provides thrust.

### Signal conditioning
This is the modification of a signal to make it more useful to hte system.
#### FIltering
This is the rejection of certain frequencies from a signal. This process removes noise from a signal.
Filters can be divided into analog and digital types.
Analog cna be divided into passive and active types. Passive filters are resistors, capasitors and inductors.

Filters can also be categorised on the type of frequecies they affect.
- Low pass filter - allow low frequencies through.
- High-pass filter - allow higher frequencies through.
- Band-pass filter allow a particular range through.
- Pand stop filter - stops  a particular range from going through.

Amplifires increase the voltage level to bettermatch the analog to dc converter range thus increasing the measurement resolution and sensitivity.

Attenuation is the opposite of amplification and decreases the input signal.
*Exitation* applying and external input to a device to make it operate. Accelerometers, thermistors and others require external voltage.
*Linearisation* this is when the sensors provide a voltage signal that is not linearly related to the physical measurement.

Some terms are:
 - linearily - how the actual measured curve of a sensor signal  departs from the dieal curve
 - Accuracy - the maximum diffeence that will exist between the actual value and the indicated value.
 - Senitivity - the minimum inout for hte physical parameter that will create a detectable output change.
 - Presision - degree of reproducability.
 - Resolution- smallest detectable incremetal change.

---
### Robotics
A robot is a mecatronic device with multiple degrees of freedom that is programmable to accomplish a variety of tasks.
*Degrees of freedom* refers to the motion capability of a robot.

Laws of robotics:
 - A robot may not harm a human being
 - A robot must obey the commands of a human being
 - A robot must protect its own existence.

Situations where robots are applied:
- Hazardous work enviroments
- repetitive work cycle
- Difficult handling such as heavy objects.
- robots are built to have a capability superior to humans such as strength or speed.
- Do not have negative human attributes such as fatigue.
![[Pasted image 20250514013617.png]]

#### Types of robots
1. Mobile robots
2. Humanoid robots
3. Parallel robots
4. Cable suspended robots
5. Soft robots

#### Robot componets
1. Transission systems - such as gears and chains 
2. Actuators - motors and pneumatic cylinders
3. Sensors - swithces and gyroscopes
4. contrillers - arduino
5. Power generation and storage - power supply units and batteries
6. Alogrithms.
7. Power generation and storage.
![[Pasted image 20250514013803.png]]

#### Input signals
Sensors detect a characteristic of the enviroment



#### Resistive sensors
- Strain gauge - used to measure strain or deformation.
- Photoresistor- used to indicate teh presence or absence of light.
- Potentiometer - it is a manually adjustable resistor used in volume control in audio equipment.
- thermistor - exhibits a change in resistance over a temprature change.

Strain gauge consist of a wire or foil patterned in a zigzag tht undergo changes in resistance when subjected to mechanical strain.
![[Pasted image 20250514015637.png]]
Compressive strain -resistance decreases
*Photoresistor*
![[Pasted image 20250514015818.png]]
*Potentiometer*
Volume control in audio equipment. Has adjustable variable resistor with 3 terminals
![[Pasted image 20250514020037.png]]



*Capacitive sensors* detect solids and liquids without physical contact. When a object comes near the sensing surface the capacitace of the oscillator changes.![[Pasted image 20250514020827.png]]
*inductive sensor* Output is in the form of inductance.
Mutual inductance is a function of the distance between the inductor and the material.
![[Pasted image 20250514021004.png]]
*Peizoelectric sensor* - electric charge that accumulates in vertain solid materials in respoce to mechanical stress. ![[Pasted image 20250514021104.png]]
#### Temprature sensors
- Bimetallic strips
- Resistance temprature detectors
- Thermocouple
- Thermodiodes and transistors

*Bimettalic sensors* Converts thermal elergy into mechanical displacement.![[Pasted image 20250514021335.png]]
*Thermocouple* - Madefrom two dissimilar metals joined in one end.
When the junction os heated or cooled it produces a voltage that can be correlated to temprature.![[Pasted image 20250514021526.png]]


### Definitions
A *system* is a combination fo compents that act together to perfomr a function.
A *model* is a formal description of a system that covers selected informationor knowledge.
*Event* is a instantanoeus occurence that chanegs the state of a system.
*Operation* is the sequence of activities that changes the stage of a system.

*System modelling* is the process of developing abstract models of a sustems with each model representing a different view of that system.
A system may be static or dynamic.
- Static - the output depents on the input variables and the present time.
- Dynamic - the output depends on the input time and the past.

There are three different kinds of systems:
 - continuous systems - one which varies with time
 - Descrete systems - observed only at strict invtervals
 - Descrete-event systems compeltely determined y a swquences of rantom times and changes in the state at that moment.