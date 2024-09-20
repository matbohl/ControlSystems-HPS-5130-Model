# ControlSystems-HPS-5130-Model
In a laboratory exercise I worked with a [HPS 5130 Motor Board](https://hps-systemtechnik.com/wp-content/uploads/content/english/5130.pdf) in connection with a [HPS 5120 PID Board](https://hps-systemtechnik.com/wp-content/uploads/content/english/5120.pdf) and measured different configurations (e.g. motor itself, closed loop control with different controllers and different loads on the motor).

To further my understanding I implemented a DC-Motor model and later the whole 5130 Board (Motor connected to generator with switchable mass and load configuration) in MATLAB Simulink and adjusted the different model parameters to match the measured behaveiour. 
The resulting setup accurately simulates the configuration on the HPS board, with dynamic friction, electrical load and changeing motor mass.

This model could be used to support future laboratory exercises and enables quickly switching between different configurations without haveing to change scaling, wires and other parts of the setup. 

What is not implemented is static friction of the motor, therefore static measurements cannot be simulated(e.g. Slowly turning up voltage until enough torque is created to overcome static friction and the motor actually starts turning).