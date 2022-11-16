This circuit allowed a z80 master and a 9995 slave processor to share the Nascom memory bus and share memory access 50:50.

The circuit plugged into the z80 socket on the Nascom board. Signal 99EN' came from keyboard port 0 bit 2
via  a flying lead. It was used to release the slave 9995 from reset and would start it from address
8000 hex - because A15 was inverted - which appeared as 0000 hex to the 9995. This was to avoid running Nas-Sys on the
9995, which would make no sense.

A similar more simple circuit - now lost - would allow two z80s to run in tandem on the Nascom. The slave z80
also started from 8000h because the top address bit was inverted. Again they time-shared 50:50 due to the action of the
steering 7474 flip-flops. When the slave was held reset, all software timings on the master were normal - but when both were
running each z80 ran half as fast, so any software timing loops ran 50% slower.

It was a fun experiment in multiprocessing.

Note: H1 to H3 signals in the circuit are just to pullup resistors

Bob Edwards G4BBY Nov 2022