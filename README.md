# Ultrasonic-sensor-with-Arduino-
The ultrasonic sensor is a device that can measure distances using sound waves . It works in a similar way than bats and dolphins - by emitting sound waves and listening them bound back . The sensor consists of two primary components: a transmitter and a receiver . The transmitter is responsible for emitting a high-frequency sound. In essence, ultrasonic refers to frequencies beyond the range of the human hearing - so something higher than 20kHz. 
When the sound wave hits an object, it bounces back like echo. This returning wave is detected by the receiver. The sensor will use the micro-controller (Arduino) internal clock to find out how much it took for the sound to bounce back. This small clock turns on when a high-frequency wave is emitted and turns off when its echo is detected. 
Using code, we can write a program that will store the timing between those two events into a variable. Then, we can use this information to calculate the distance between the sensor and the object. 
You may be thinking: how can we find the distance if all we know is the timing? 
Well, as you know, velocity is distance divided by time. Based on this equation, if we multiply the velocity by the time, we'll find the distance . I told you the sensor emits sound waves, so the velocity we need is the speed of sound in air (340 m/s). 
Velocity = Distance / Time 
Distance = Velocity * Time 
But if we multiply this speed with the timing we found, we'll discover a value that's twice the real distance. That's happens because the sound hit the object and came back, in other words, it traveled the same path twice. Then to find the real distance, multiply the speed of sound with the timing and divide the result by two. 
Distance = (Velocity * Time) / 2 
The sensor consists of two primary components: a transmitter and a receiver . The transmitter is responsible for emitting a high-frequency sound. In essence, ultrasonic refers to frequencies beyond the range of the human hearing - so something higher than 20kHz. 
When the sound wave hits an object, it bounces back like echo. This returning wave is detected by the receiver. The sensor will use the micro-controller (Arduino) internal clock to find out how much it took for the sound to bounce back. This small clock turns on when a high-frequency wave is emitted and turns off when its echo is detected. 
Using code, we can write a program that will store the timing between those two events into a variable. Then, we can use this information to calculate the distance between the sensor and the object. 
You may be thinking: how can we find the distance if all we know is the timing? 
Well, as you know, velocity is distance divided by time. Based on this equation, if we multiply the velocity by the time, we'll find the distance . I told you the sensor emits sound waves, so the velocity we need is the speed of sound in air (340 m/s). 
Velocity = Distance / Time 
Distance = Velocity * Time 
But if we multiply this speed with the timing we found, we'll discover a value that's twice the real distance. That's happens because the sound hit the object and came back, in other words, it traveled the same path twice. Then to find the real distance, multiply the speed of sound with the timing and divide the result by two. 
Distance = (Velocity * Time) / 2 
Project
In this article, I will show you how to build an alarm system using Arduino and the ultrasonic sensor. If you don't have all components or would like to test before assembling anything, I created a simulation of this alarm system on Tinkercad . You can run it directly on your browser by clicking $ here $ . 
Moving on, for this project, you'll need: an Arduino board, a breadboard, a bunch of jumper wires, a buzzer,and an ultrasonic sensor. 
