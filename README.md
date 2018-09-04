# TopPASS-RWD
TopPass NFC Re-Writer SICRE31/41 firmware for Arduino

This RWD was designed for demostration of "TopPASS" - NFC Smart Ticketing System. 
There are tree kinds of operational modes:

- Ticket Validation Mode (Mode 1):
    - Initailzed by STAFF wristband, and load EVENT access pass to RWD.
    - STAFF wristband created by WASHOW adminstration pass (4Bytes).
    
- Cashless Payment Mode  (Mode 2):
   - According to EVENT pass to check the balance of TopPASS ticket.
   - Automatic "TopUP" to 250 pt. was enable when insufficient balance was occurred.
   - Each tap will display balance first, and keep ticket in-the-field at least 1.5 sec. deduct 50 pt. one times.
   
- Security Guard Mode  (Mode 3):
   - Turn ON the R/W memories protection from addr.0x20
   - Two kinds of tag ICs, SIC43NT and NTAG213, were supported.
