This submission is for not being automatically revoked by mistake by system of Udacity based on the advise of our instructor that the deadlines doesn't meet actual deadlines of the projects.

hope to finish the project and hand it soon.

components:
  two microcontrollers
  connect via CAN.
  one door sensor.(D)
  one light switch.(L)
  one speed sensor.(S)
  Two light sources:
    Right(RL).
    Left(LL).
  One Buzzer(B).
  ECU 1 connected to D, S, L, and any input device.
  ECU 2 connected to RL, LL, and B and all output devices.
  
Requirements:
  1- ECU1 will send status massages periodically to ECU2 through CAN protocol.
  2- Status massages will be sent using Basic communication module(BCM).
  3- Door state massages will be sent every 10ms to ECU2.
  4- Light switch state massage will be sent every 20ms to ECU2.
  5- Speed state massage will be sent every 5ms to ECU2.
  6- each ECE has an OS and application SW components.
  7- OUTPUTS:
      Car     Door     Light_Switch|   Buzzer  Light                    
      move    OPEN     X           |   ON      OFF
      STOP    OPEN     X           |   OFF     ON 
      X       CLOSE    X           |   X       OFF after 3 seconds
      Moving  X        ON          |   OFF     ON 
      STOP    X        ON          |   ON      ON   

using binary math 
buzzer is on iff car is stop and light_switch is on (cL) or moving and open (Cd).
Light: switch on or door open and car stop


Static design:
    ECU 1:
        Make layered architecture.
        specify modules of the comp.
        full details of API for modules.
        details of typedef used.
        prepare folder structure for previous points.
    
    ECU 2:
        Make layered architecture.
        specify modules of the comp.
        full details of API for modules.
        details of typedef used.
        prepare folder structure for previous points.
            
provide pdf containing all work.
a video where you discuss your work (max 3 min).


Dynamic design:
      ECU1:
        Draw state machine diagram of the comp.
        Draw state machine diagram of the operation.
        Draw the sequence diagram of the ecu.
        calculate the CPU load for the ECU.
      ECU2:
        Draw state machine diagram of the comp.
        Draw state machine diagram of the operation.
        Draw the sequence diagram of the ecu.
        calculate the CPU load for the ECU.
          Load represents the percentage of system bus busy per second.

provide pdf containing all work.
a video where you discuss your work (max 5 min).



