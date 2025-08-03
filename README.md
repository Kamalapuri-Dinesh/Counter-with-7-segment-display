3-Digit 7-Segment Display Counter with Arduino

This project displays numbers from 0 to 150 using three 7-segment displays and an Arduino UNO or Nano. The numbers are multiplexed to reduce the number of required I/O pins.

 Hardware Used

 1. Arduino UNO / Nano -1
 2. 7-Segment Displays -3
 3. 300Ω Resistors -3

 Circuit Description

- Segment Pins (A to G) of all displays are connected in parallel to Arduino D2 to D8.
- Common cathode (COM) pins of each display are connected through 300Ω resistors to:
  - Hundreds → A2  
  - Tens → A1  
  - Units → A0  
- Resistors protect the display from overcurrent.
- Only one digit is activated at a time using multiplexing.

Working Principle

This project uses multiplexing. All segment pins are shared, but only one display is activated at a time for a short period. The display is fast enough that the human eye sees all digits on at once.


