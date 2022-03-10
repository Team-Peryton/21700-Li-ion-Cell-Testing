# Lithium Ion Cell Testing

Collecting data using a powerlab8 V2 charger. Capable of 60A discharge to a battery supply, 10A internal dissipation.

Cells tested -> Molicell INR-21700-P42A.

## Aims
- check cell capacity variance
- check cell internal resistance variance
- understand optimal cell cutoff voltage for our current draw
- measure cell response to a 60a 10 second current draw

## Repo contents
- [ ] raw cell data
- [ ] script to process raw data into useful things
- [ ] summary excel sheet once all data has been collected
- [ ] discharge plots 

## data

test data in native PowerLab 8 V2 software format (.CP8) as well as tab separated format (.txt)

- N_cell_cycle.*      :   (charge to 100% SoC if needed) discharge at 1C then charge at 1C
- N_cell_storage.*    :   Discharge from 100% SoC to 3.7V storage charge at 10A, ~2.4C
- N_cell_stress.*     :   Discharge from 100% SoC to 4.0V (TBC) at 60A, ~14C
