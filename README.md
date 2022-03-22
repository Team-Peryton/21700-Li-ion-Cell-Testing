# Lithium Ion Cell Testing

Collecting data using a powerlab8 V2 charger. Capable of 40A discharge to a battery supply, 10A internal dissipation.

Cells tested -> Molicell INR-21700-P42A: https://www.imrbatteries.com/content/molicel_p42a.pdf

Can get the Revolectrix CCS PowerLab 8 software here: https://www.rcgroups.com/forums/showthread.php?3963135-Revolectrix-CCS-Install-Workaround#post47730189


## Aims
- check cell capacity variance
- check cell internal resistance variance
- understand optimal cell cutoff voltage for our current draw
- measure cell response to a 60a 10 second current draw

## Repo contents
- [X] data/set1 raw cell data - test setup introduced apparent cell to cell variance - systematic errors in internal resistances ?
- [ ] data/set2 raw cell data - test setup improved (awaiting results)
- [X] script to process raw data into useful things
- [X] set 1 summary excel sheet
- [ ] set 2 summary excel sheet
- [X] set1 plots
- [ ] set2 plots

## data

test data in native PowerLab 8 V2 software format (.CP8) as well as tab separated format (.txt)

- N_cell_cycle.*      :   (charge to 100% SoC if needed) discharge at 1C to 2.5V, 1 min rest, then charge at 1C to 100% SoC
- N_cell_storage.*    :   Discharge from 100% SoC to 3.7V storage charge at 10A, ~2.4C
- N_cell_stress_XA.*  :   Discharge from 100% SoC to 4.0V (TBC) at X Amps, ~14C

![hi](/cells.jpg)