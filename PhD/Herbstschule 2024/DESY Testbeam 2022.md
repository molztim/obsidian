# Test Parameters

- Positions between 1.4 GeV and 5.4 GeV

# Test performance

### Refelctivity

- Around 65% due to rust.
- Improvements in Sciitllator purification, WOM Coating, WOM-SIPM coupling and Cell wall refelctivity were done here
- Methode to calcualte Refelcitivity: 
	- Simulate detector in MC simulation with the same particles, energies and electronics, but variable wall refelctivities.
	- A set of 7 simulations with differenct refelctivities yield different average photon yields.
	- These yields were directly compared to the measured avergae integrated yield form the test beam by employing a scaling parameter depending on the refelctivity.
	- A chi2 analysis yielded an optimal simulation for 65% reflectivity.
- The procedure was repeated for different angles, positions and energies to validate the analysis. 
	- The yield increases with higher angles, since the paritcles travel through more scintilaltor.
	- The yield decreases the further the point of interaction is from the WOM.

### Detection effiency

- Above 99.3% at 68% confidence level for whole cell
- Above 99.5 % at 68% confidence level for at least one of two WOMs
- Methode:
	- Effiency was calculated by calculating the charge spectrum of our detector for given energies and then apllying a cut to seperate dark-counts from event.s
	- The charge spectrum is a histogram of the total charge deposited by a particle inside the detecotr. This can be calculated by integrating the waveform of an event. All integrals are then merged into a histogram.
	- A seperate measurement without a beam was run to detemine the charge specturm of dark counts. This spectrum allowed us to detemine a upper limit for the charge geenrated in dark counts (800 mVxns).
	- We then cut the charge spectrum from the data with this limit and caculated the ratio of the remaining data to the total data.
	- Since the WOMS behave differently, we assumed the worst possible case (far from WOM, low beam energy) for alower limit. This was at larger than 99.3% with 68% confidence level. 
	- Now since we have two WOMs in one detector, we need to consider that one or both WOMs have seen the event for the total detector effiency. This raises the lower limit to 99.5% at 68% confidence level.

### Particle Crossing Point

- NN approach: below 14cm

### Energy Response

- Mehtode:
	- One angle, multiple position and angle.
	- Sum up waveforms for each event (surression of noise) and apply smoothening.
	- Then figure out Time where the smoothend, summed waveform reaches 25% peak amplitude (constant fraction discrimination)
	- Get two times: Td for fown-WOM and Tu for up-wom
	- The calculate average arrival time of our four trigger PMTs inmto the trigger time Ttrigger, with the same 25% threashold
	- Calculate time uncertainty of trigger from time distribution of PMTs (~0.1ns)
	- Correct Tu and Td with trigger time Ttrigger to eleminate time offsets between differnet events
	- Do for different positions - vary of Tud ist 2ns. 
	- This is the intrinsic time variation.
	- Statistical uncertainty from the data below: 0.8ns
	- Afterwards: Likelihood correction for non-uniformity of integrated light yield in detector. Similar l
- Intrinsic time variation: Calculated from spread of the range of the averages of the corrected arrival time at Woms to be 2ns
- Result: Resolution is +- 1ns
- Improvement of statistical fluctuation by increasing lightyield
- WHAT DOES THE LIKELIHOOD CORRECT?

# Fragen an Horst