     PCB NO: XXXXXX-XX VER.X
DESCRIPTION: <ENTER DESCRIPTION FROM AS400 HERE>


GERBER PHOTOPLOT FILE SETTINGS:
1. UNITS = INCHES
2. FORMAT = 2.4 (TWO DIGITS RIGHT AND FOUR DIGITS LEFT)
3. LEADING AND TRAILING ZEROS (NO ZERO SUPPRESSION)
4. POSITIONED RELATIVE TO ORIGIN
5. ALL FILE VIEWS ARE LOOKING THROUGH THE CIRCUIT BOARD FROM THE TOP.

    FILES REQUIRED FOR MANUFACTURING BLANK PCB
|-------------------------------------------|------------------------------------|
|              FILE DESCRIPTION             |              FILE NAME             |
|-------------------------------------------|------------------------------------|
|   DRILL REPORT                            |       PANEL XXXXXXXX.DRR           |
|-------------------------------------------|------------------------------------|
|   INNER COPPER LAYER 1                    |       PANEL XXXXXXXX.G1            |
|-------------------------------------------|------------------------------------|
|   INNER COPPER LAYER 2                    |       PANEL XXXXXXXX.G2            |
|-------------------------------------------|------------------------------------|
|   BOTTOM COPPER LAYER                     |       PANEL XXXXXXXX.GBL           |
|-------------------------------------------|------------------------------------|
|   BOTTOM OVERLAY (SILKSCREEN)             |       PANEL XXXXXXXX.GBO           |
|-------------------------------------------|------------------------------------|
|   BOTTOM SOLDERMASK                       |       PANEL XXXXXXXX.GBS           |
|-------------------------------------------|------------------------------------|
|   PANEL OUTLINE                           |       PANEL XXXXXXXX.GM2           |
|-------------------------------------------|------------------------------------|
|   PANEL V-SCORE                           |       PANEL XXXXXXXX.GM3           |
|-------------------------------------------|------------------------------------|
|   PANEL CUTOUTS                           |       PANEL XXXXXXXX.GM4           |
|-------------------------------------------|------------------------------------|
|   VENDOR MARKING AREA                     |       PANEL XXXXXXXX.GM7           |
|-------------------------------------------|------------------------------------|
|   TOP COPPER LAYER                        |       PANEL XXXXXXXX.GTL           |
|-------------------------------------------|------------------------------------|
|   TOP OVERLAY (SILKSCREEN)                |       PANEL XXXXXXXX.GTO           |
|-------------------------------------------|------------------------------------|
|   TOP SOLDERMASK                          |       PANEL XXXXXXXX.GTS           |
|-------------------------------------------|------------------------------------|
|   NC DRILL FILE (HOLES)                   |     PANEL XXXXXXXX-HOLES.TXT       |
|-------------------------------------------|------------------------------------|
|   NC DRILL FILE (SLOTS)                   |     PANEL XXXXXXXX-SLOTS.TXT       |
|-------------------------------------------|------------------------------------|



    FILES REQUIRED FOR ASSEMBLING PCB
|-------------------------------------------|------------------------------------|
|              FILE DESCRIPTION             |              FILE NAME             |
|-------------------------------------------|------------------------------------|
|   ASCII SOURCE FILE (NOT PANELIZED)       |    ASCII PCB XXXXXXXX.PcbDoc       |
|-------------------------------------------|------------------------------------|
|   TOP ASSEMBLY                            |        PANEL XXXXXXXX.GM5          |
|-------------------------------------------|------------------------------------|
|   BOTTOMSEMBLY                            |        PANEL XXXXXXXX.GM6          |
|-------------------------------------------|------------------------------------|
|   TOP SOLDER PASTE                        |        PANEL XXXXXXXX.GTP          |
|-------------------------------------------|------------------------------------|
|   BOTTOM SOLDER PASTE                     |        PANEL XXXXXXXX.GBP          |
|-------------------------------------------|------------------------------------|
|   PICK AND PLACE (CENTROID)               |     PICK PLACE PANEL XXXXXXXX.CSV  |
|-------------------------------------------|------------------------------------|
|   PICK AND PLACE (ALTIUM OUTPUT)          |     PICK PLACE PANEL XXXXXXXX.TXT  |
|-------------------------------------------|------------------------------------|

NOTE: Altium added some extra parameters to the ASCII outputs in v18 that the
      AEGIS software (used by some of our vendors) wasn't expecting to see. This
      is causing the Aegis software to fail to load the ASCII board files. This
      has been confirmed by several other users on the Altium message boards. The
      current workaround when doing designs in v18 is to generate the ASCII board
      files from v17.
                                                        