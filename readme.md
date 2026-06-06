# Setup

Clone the repo into  

```
~/linuxcnc/configs/
```

Set a static IP for the computer:
192.168.2.1



# Useful Commands

halcmd interactive
$ halcmd -kf

halcmd: 
    show 
    show pin
    


registers that are working

write that works:
    mbpoll -m rtu -a 1 -b 4800 -P even -t 4:int -r 1       -1 /dev/ttyUSB0 0x0000
read that works:
    mbpoll -m rtu -a 1 -b 4800 -P even -t 4:int -r 16 -c 1 -1 /dev/ttyUSB0




Spindle Information:
Min Rated Speed: 
Max Power Speed: 12000 (12kw / 16HP)    
Max Speed:       24000                  800 Hz


Warm Up:
-  50% Speed  2 min   (12000 RPM) (200 RPS) (400 Hz)
-  75% Speed  2 min   (18000 RPM) (300 RPS) (600 Hz)
- 100% Speed  1 min   (24000 RPM) (400 RPS) (800 Hz)


