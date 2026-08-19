Hours covered in this Journal: 5hrs <br>
Now that i had completed the ideation part of it, i started building the schematic. so i built 2 projects,<br>
the left and the right keyboards, and though i will just flip them. (I was wrong, will cover this later). <br>
I built the basic switch<img width="268" height="223" alt="Screenshot 2026-08-18 194559" src="https://github.com/user-attachments/assets/21dbd56c-c027-4581-a565-51b07c3072e7" />
<br>
and then started to place the rest in the layout i had planned<br><img width="434" height="236" alt="Screenshot 2026-08-18 195150" src="https://github.com/user-attachments/assets/dc90c9fc-2433-455c-91ac-91d5d047324b" />
<br>
the gimmick is the joystick for both thumbs and the oled and rotary wheels for the left side, but since they were at a different place as compared to the rest of the pcb, i added solder wire pads to route the wires physically with solder.
<br> This was also done for the 4 thumb buttons.
<br>
<br>
Next up was the Pi pico, and i decided to use a audio jack to connect the 2 halves using UART, and wired the rows, cols, oleds and everything else. I had to shift the pins later on to make the pcb simpler tho.
<br> <img width="667" height="475" alt="image" src="https://github.com/user-attachments/assets/6b4e77bd-50ef-447c-87cf-e4808a59477f" />
<br> the layout is as follows: the picos communicates through master slave network using TRRS(fancy way of saying using the audio cable to transfer data instead of audio). the picos have their tip and ring 1 connections swapped so as to make the proper receiving and transmitting pairs. The joystick is a standard ps4-esque joystick with 5v input and x y and switch outputs. The oled and the rotary wheel both have 3v input.<br>
<img width="910" height="582" alt="image" src="https://github.com/user-attachments/assets/dcb883b9-bcc9-4956-a8a8-93ad2b9d6c12" />
i did all this for both the split sides on separate kicad projects, but the oled and rotary will only be on the left side.
