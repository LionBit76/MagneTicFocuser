# MagneTicFocuser
DIY focuser for astrophotography with a magnetic flange

My Blogpost (german): https://astrophoto.lionbit.com/3d-druck/22-magneticfocuser

![This is an image](https://github.com/LionBit76/MagneTicFocuser/blob/main/images/MagneTicFocuser_PG27.png)

When I was looking for a cheap way to get a focuser, I came across a project on GitHub called TicFocuser-NG. This is an INDI driver for a Pololu TIC Controller. This controller is a small, compact circuit board with a stepper motor driver and a controller that is addressed via MicroUSB. The advantage of this solution is that you don't need an Arduino or Raspberry Pi to control the stepper motor driver, everything is on a board that is smaller than the area of a NEMA17 motor.

This focuser is for astrophotography with the INDI driver TicFocuser-ng https://github.com/sebo-b/TicFocuser-ng

### BOM [MagneTicFocuser]:

- 1x STEPPERONLINE 17HS13-0404S-PG27 
- 1x Pololu Tic T500 
- 4x M3x6 for fastening the geared motor 
- 4x M3x10 for the connection between housing and magnet plate
- 2x M2x8 self-tapping for attaching the controller
- 2x M4x10 grub screw for the clutch
- 4 N54 neodymium magnets 9x5 (4 more for the flange on the telescope)
- 1x barrel connector socket 5.5x2.1 for 12V DC
- 4x heatset inserts M3 5x6 (I have the VORON compatible heatset inserts)
- Superglue to stick the magnets in place
- JST connectors 4-pin for stepper, 2-pin for 12v

### Motor settings:
My settings in the Tic Software for the stepper motor are:
- Current limit: 1mA (yes, it works!)
- Step mode: 1/8 step (for maximum resolution and less vibrations on accel/deccel)
- Max speed: 8000000
- Max accel: 80000

### MagneTicFocuser and Explore Scientific ED80:
![This is an image](https://github.com/LionBit76/MagneTicFocuser/blob/main/images/MagneTicFocuser.jpg)

### MagneTicFocuser mounted on Explore Scientific ED80:
![This is an image](https://github.com/LionBit76/MagneTicFocuser/blob/main/images/MagneTicFocuser_mounted.jpg)



This project started on 2022-06-25 and it is still under development...
