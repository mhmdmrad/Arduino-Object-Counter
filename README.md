# DONE
# Arduino Digital Object Counter 

## Project Overview  
This is an Arduino-based **Digital Object Counter** that counts objects passing in front of an IR sensor.  
The count is displayed in real-time on a 16x2 LCD, with a buzzer providing audio feedback on detection.  
A push button allows the user to reset the count to zero.  

## Features  
- **Object Detection:** Counts objects using an IR sensor.  
- **Real-Time Display:** Shows the count on a 16x2 LCD.  
- **Buzzer Feedback:** Beeps briefly when an object is detected.  
- **Reset Button:** Resets the object count to zero.  

## Components Used  
- Arduino Board  
- IR Sensor  
- 16x2 LCD Display (I2C)  
- Buzzer  
- Push Button  
- Jumper Wires and Breadboard  

## Wiring  

| **Component**    | **Arduino Pin**               | **Details**                      |  
|------------------|-------------------------------|----------------------------------|  
| **IR Sensor**     | Pin 2                         | Detects objects passing in front |  
| **Buzzer**        | Pin 3                         | Provides beep feedback           |  
| **Push Button**   | Pin 4                         | Configured with `INPUT_PULLUP`   |  
| **LCD Display**   | I2C Communication (0x3F)      | 16x2 LCD via I2C interface       |  

## Code Functions  
- **`setup()`** – Initializes the pins and LCD display.  
- **`loop()`** – Handles object detection, updating the count, and resetting.  
- **`Count()`** – Increments the counter, updates the LCD, and triggers the buzzer.  
- **`Reset()`** – Resets the count to zero and refreshes the LCD.  

## How to Use  
1. **Upload the code** to your Arduino board.  
2. Connect the components according to the wiring guide.  
3. Power the system and start counting objects!  
4. Press the push button to reset the count.  

## Applications  
- People counting at entrances/exits.  
- Object counting on conveyor belts.  
- Inventory tracking in warehouses.  
