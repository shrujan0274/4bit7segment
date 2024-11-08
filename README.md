# Design And Implementation of a Seven Segment Display Controller Using a 4-bit Binary Input
Shrujan Karthik V <br>
Department Of Electronics And Communications Engineering<br>Sri Eshwar College Of Engineering, Coimbatore-641202<br>
shrujanemerging@gmail.com
 # Glance
<pre>This combinational circuit is designed to operate the seven-segment display using its 4-bit binary/BCD input. The circuit is designed in such a way that the selective segments are only operated for a particular input by displaying the numbers exactly. This system takes 4-bit input as the signal operates the combinational circuit accordingly, and gives seven outputs ranging from A to G to control the segments A to G. The combinational circuit is designed entirely using transistors and logic gates. </pre>
This project investigates the design and implementation of a seven-segment display controller which is operated by 4-bit binary or BCD code input. This is a simple combinational Circuit that can also be integrated with a sequential circuit for an automation process.<br>
This circuit takes 4-bit input and a total of 7 outputs which is used to control the seven segments in the seven-segment display. At the elementary level, this circuit is designed only as a combinational circuit. This circuit can be further utilized by connecting it to a counter. The counter output can be converted into the BCD code using a binary code to BCD code converter. This can also be used in several applications. This can also be connected to registers using a binary-to-BCD code converter and to the seven-segment display. The elementary design is made in such a way that 4-bit binary input and BCD input can also be given to the controller to display the output in the seven-segment display. Since the 4-bit Binary ranges from 0-15 and the seven-segment display can be only used to display 0-9 it can be used to display 0-9 using the input since the BCD code and the 4-bit binary code are the same for the inputs 0-9. For inputs 10-15 in binary, the system is designed in such a way that for inputs ranging from 10-15 in binary, the display shows nothing as the output, i.e. all the seven segments of the display are kept off. <br>
Currently, we are going to design and implement only the seven-segment display controller in this entire block diagram. One of the important applications of this controller is this can be used in the Number Guessing Game by using only the controller and by giving the binary input manually using push-switches. For inputs that are larger than 10, we need to design the binary to BCD converter accordingly so that we can use four outputs for each seven-segment display, and we need to use one separate controller for each BCD code output. So we need to use separate controllers for every seven-segment Display.

# Block Diagram
![Block Diagram](https://github.com/user-attachments/assets/7074bd06-2202-4df2-9c21-15906c99d7fd)
# Circuit Diagram Of The Controller
![Circuit](https://github.com/user-attachments/assets/db5023a9-bcc9-46c9-9364-b13172b9e05a)
# Working Parameters
|parameter|description|min|type|max|unit|condition|
|---------|-----------|---|----|---|----|---------|
|Technology|180nm CMOS process||||||
|RL|Load Resistance At Input Terminals|100|||MOhm|VDD=5V Temp=27C|
|CL|Load Capacitance At Input Terminals|||30|pf|VDD=4.5-5V Temp=30-100C RL=100M|
|Input V|Input Voltage|0|4.5|5|Volts|Temp=27C|
|Supply V|Supply Voltage|4.5|4.75|5|Volts|Temp=27C|

