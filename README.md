# IO4-QuadOD
## License: CERN Open Hardware Licence v1.2

IO4 Quad Detector for DCCOD and CPod detector cards


This project is a simple baseboard for current sensing detectors.
It was inspired (in reverse chronological order) by railnerd, MarkS, MRCS, RR-Cirkits and, of course, Dr Bruce Chubb.


This is a multi-purpose board - it supports 3 different use cases:


1. It can be an IO4 peripheral using the SPCoast 6-pin RJ12 connector scheme,
2. It can be hardwired using screw terminals and/or a 5VDC wallwart, or
3. With the addition of a WemosD1Mini 8266 MCU board, it can become a distributed WiFi and/or I2C peripheral. (Software TBD)


The MRCS CPod and the CMRI DCC-OD detectors both work with this baseboard.

The 2x IO4 connections are arranged so that two adjacent control
points can both monitor a shared set of detected blocks (usually
used by approach logic...).  One (master) provides a power source,
the other (slave) does not; all other signals from the IO4 connector
are in common.  This implies that both need to be connected to INPUT
configured ports.





