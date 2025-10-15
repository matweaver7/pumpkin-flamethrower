# Pumpkin Flamethrower

Ever wanted a super dumb and dangerous pumpkin that shoots flames out of it's mouth? Yeah. Me neither. But here it is anyway.

### Design


```
 +-------------------------+
          |       5V Adapter        |
          |   (5V 2A or 3A output)  |
          +-------------------------+
                |             |
                |             |
                |             +--------------------+
                |                                  |
                v                                  v
           +---------+                       +-----------+
           |  ESP32  |                       |  Servo    |
           |         |                       |  (5V type)|
           +---------+                       +-----------+
              | 3.3V logic                         |
              |                                    |
              |                                    |
  GPIO 13 ----+-----------------------> Servo Signal (orange/yellow)
   (or any PWM pin)
              
  GND -------------------------------> Servo Ground (brown/black)
   (shared common ground!)

  5V pin <---------------------------- Servo Power (red)
     ^  
     | (optional)
     | can be fed by same 5V adapter if it’s 2A+ rated
```
