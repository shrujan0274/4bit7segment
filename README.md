# Design And Implementation of a Seven Segment Display Controller Using a 4-bit Binary Input
Shrujan Karthik V <br>
Department Of Electronics And Communications Engineering<br>Sri Eshwar College Of Engineering, Coimbatore-641202<br>
shrujanemerging@gmail.com
# Glance
<div style="text-align: justify;">
This combinational circuit is designed to operate the seven-segment display using its 4-bit binary/BCD input. The circuit is designed in such a way that the selective segments are only operated for a particular input by displaying the numbers exactly. This system takes 4-bit input as the signal operates the combinational circuit accordingly, and gives seven outputs ranging from A to G to control the segments A to G. The combinational circuit is designed entirely using transistors and logic gates. <br><br>
This circuit takes 4-bit input and a total of 7 outputs which is used to control the seven segments in the seven-segment display. At the elementary level, this circuit is designed only as a combinational circuit. This circuit can be further utilized by connecting it to a counter. The counter output can be converted into the BCD code using a binary code to BCD code converter. This can also be used in several applications. This can also be connected to registers using a binary-to-BCD code converter and to the seven-segment display. The elementary design is made in such a way that 4-bit binary input and BCD input can also be given to the controller to display the output in the seven-segment display. Since the 4-bit Binary ranges from 0-15 and the seven-segment display can be only used to display 0-9 it can be used to display 0-9 using the input since the BCD code and the 4-bit binary code are the same for the inputs 0-9. For inputs 10-15 in binary, the system is designed in such a way that for inputs ranging from 10-15 in binary, the display shows nothing as the output, i.e. all the seven segments of the display are kept off. <br><br>
Currently, we are going to design and implement only the seven-segment display controller in this entire block diagram. One of the important applications of this controller is this can be used in the Number Guessing Game by using only the controller and by giving the binary input manually using push-switches. For inputs that are larger than 10, we need to design the binary to BCD converter accordingly so that we can use four outputs for each seven-segment display, and we need to use one separate controller for each BCD code output. So we need to use separate controllers for every seven-segment Display. <br>
</div>

# Block Diagram
![Block Diagram](https://github.com/user-attachments/assets/876d0fbe-7996-46cc-a9f8-e1a22f069f74)
# Circuit Diagram Of The Controller
![Circuit](https://github.com/user-attachments/assets/d4aabe2f-9aa7-448b-a5a2-ec45ac6eb6aa)
# Working Parameters
|parameter|description|min|type|max|unit|condition|
|---------|-----------|---|----|---|----|---------|
|Technology|180nm CMOS process||||||
|RL|Load Resistance At Input Terminals|100|||MOhm|VDD=5V Temp=27C|
|CL|Load Capacitance At Input Terminals|||30|pf|VDD=4.5-5V Temp=30-100C RL=100M|
|Input V|Input Voltage|0|4.5|5|Volts|Temp=27C|
|Supply V|Supply Voltage|4.5|4.75|5|Volts|Temp=27C|
|Output V|Output Voltage|0||5|Volts|Temp=27C VDD=4.5-5V Input V=0-5V|

# Issues And Improvements Made
While designing most of the systems are designed by considering the inputs ranging from 10-15 as don’t care. While considering it as don’t care, they are also grouped in the k-map while designing. Due to the inputs ranging from 10-16, the seven-segment display shows meaningless output. That issue is solved in the current system by designing in such a way that all the seven segments should be turned off while the inputs ranging from 10-15 are given to the input. This is one of the major improvements made in the current design. This system is also useful when the BCD code converter fails and gives an invalid output the display shows nothing and the problem can be identified very easily.
# Future Works
This system lays the foundation for the various applications that use the seven-segment display. By using a counter and clock and various other combinational and sequential circuits, a digital clock can be designed with this circuit as a base.
# References
1. SN74LS47 - BCD-to-Seven-Segment Decoders / Drivers - Texas Instruments - https://www.ti.com/lit/ds/symlink/sn74ls47.pdf?ts=1730217589708&ref_url=https%253A%252F%252Fwww.ti.com%252Fproduct%252FSN74LS47
2. Design of an electronic watch M. Liakot Ali; R. Sanusi, Wan Azib Wan Adli - https://ieeexplore.ieee.org/document/1033115
3. An Effective Approach to Designing Seven Segment Static Display Systems with Complete Character Representation - Ezekwe Chinwe Genevra, Okwu Patrick Ikechukwu, Mbonu ekene Samuel, Ude Nnaemeka Godwill - https://www.researchinventy.com/papers/v3i12/I0312050058.pdf
# Contributors
Shrujan Karthik V

# Acknowledgements
- Sree Vishnu Varthini S, Department of Electronics And Communication Engineering, Sri Eshwar College Of Engineering, Coimbatore
- Vijay N, Physical Design Engineer, Tech Mahindra Cerium
- Akash E, Intern, Analog Layout Engineer, Cadence Design Systems
- Mr.Saravanan M, Assistant Professor, Head COE-System On Chip, Department of Electronics And Communication Engineering, Sri Eshwar College Of Engineering, Coimbatore
- Dr.Babu Karuppiah A, Professor, Department of Electronics And Communication Engineering, Sri Eshwar College Of Engineering, Coimbatore
- Dr.Shanmughasundaram N, Professor And Head, Department of Electronics And Communication Engineering, Sri Eshwar College Of Engineering, Coimbatore
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.
# Contact Information
- Shrujan Karthik V <br>
Email<br>
Personal : shrujanemerging@gmail.com<br>
College : shrujankarthik.v2023ece@sece.ac.in
