# Bob-Edwards--Polydos programs
Blue Label Pascal v1.3, adapted to

1. Load and Save source files from Polydos disk
2. Save compiled programs to disk
3. Compiled programs can be run from the Polydos prompt

blpascal.img is a disk image containing:-
Sect   Nsec    Load    Exec   Name        Comment
0004   0031    1000    4000   DPASCAL.GO  BL Pascal v1.3 with disk extension
0035   0041    0000    0000   PAfh.TX     Disk extension overlay - source code
0076   0006    C800    0000   PAfh.OV     Disk extension overlay
007C   002A    0000    0000   VGRA.TX     Pixel Graphics overlay - source code
00A6   0004    C800    0000   VGRA.OV     Pixel Graphics overlay
00AA   000A    0000    0000   BUBBLE.TX   Graphics demo for circles
00B4   000C    0000    0000   CUBIC.TX    Graphics demo for points and lines
00C0   0001    0000    0000   TEST.TX     Simplest pascal program for initial test

     
