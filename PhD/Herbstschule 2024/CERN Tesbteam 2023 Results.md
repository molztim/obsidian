# Test Goals

- Study particle reconstruction for particles crossing multiple cells
- Study reflectivity from new anti-rust primer in paint

# Testbeam Parameters

- Muon Beam at T9 at CERN

# Testbeam Results

- A lot is still WiP

### Time perfromance

- Copared time performance for Wavecatcher ADC with simulated ToT (5mV) ADC
- Simulated: Take wavectacher data and simulate ToT ADC by coutning the data above the threshold form wavectatcher data.
- Point: ToT ADCs are more feasable for the experiment then using Sampling ADCs
- With wavecathcer: Integrate waveform for each SIPM channel (over time)
- Time-integrate the sum of alll waveforms for one WOM
- Calculate time differneces bteween WOMs to get travel time between trigger and WOM away
- With ToT: take time over threhsold for each channel
- Calculate differneces between WOMs
- RESULT: Similar performances! ToT concept pooved value


### Reflectivity

- LS transaprency degraded due to air contact when opening filled cell for interventions
- LS was also degraded by Rust form cell walls.
- Rust started to form even with the new primer, degrades LS, re-purification ist expensive
- Spray coating is expensive, takes long, requires special infrastructure and is itme consuming
- AlsoBaSO4 paint aged faster than expected.
- Bottom Line: Need to get rid of the paint.
- Solution: use metal for box witht e highest UV reflectivity

### Electronics response

- Measured Darkcount charge spectrum by deactivaigt beam and beam telescope
- Calculated charge spectrum from events, fitted single photon events (1PE), zero photon events (0PE, aka electronic noise) and two photon event (2PE) curves spectra to extract single photon probability and gain single photon waveforms
- 0PE: order ofmagnitutde of 0.6mV, can apply cut here!
- 1PE: DC ~64%, I believe that 64% of all events are Dark Counts
- 2PE: Defines the Crosstalk Prob ~ 10%
- No after pulse implemented yet
- Compare data to MC simulation of average waveform (for one event.) Includes:
	- LY from scinitllator and kinetcs
	- Light propagation: LS transperency, wall reflectvity, PMMA vessel transperency, WOM absoprtion, transport in WOM to SIPM, SIPM photodetectionefficiency
	- SImulation with 1PE
	- Cross-talk and dark countsa ddede
	- missing afterpulsing

### Photon transportation

- Simulation vs data from 4 cell prototype
- Simulation: Contains full simulation from muon energy to SIPM waveform
- Assumed reflectivity: 96% - 98%
- Agrees with WOM close to lightsource, overestimates WOM far from light source. 
- We measured at CERN a reflectivity with fresh paint >96%. With a 1-year old BaSO4, the reflectiviy dropepd already ~ 80%. We see a quite powerfull ageing. 


### Extra: Light Yield (LY)

- Primary LY: PPO conecntration (plan on increasing)
- LAB+PPO transparency in the UV. Affected by LAB purity and ageing.
- Cell-Wall reflectivity: LY ~ R² (R: Relfexionsfaktor, dieser ist die größe, der an die AMplitude gekoppelt ist)
- WLS layer thickness (more thickness, more chance of conversion), already coated both sides
- WOM transparency (i.e. how UV transparent is the PMMA)
- SiPM geometrical cover: how much surface does the SiPMs cover from the WOM end
- SiPM PDE - obviously
- Optical coupling SIPM to WOM: requires much optimization


# Questions

1. Warum wird bei der time performance bei ToT ebenfalls die summe über die integrale gebildet?
2. Was ist die Likelihood alanyse für die zeit korrektur für die eintritts punkte?
3. Wie habe wir nochmal den random trigger gemacht?
4. Was ist die DC probability bei 1PE? 10% of all dark counts produce crosstalk? That looks high
5. Was genau wollen die jetzt untersuchen mit dne Daten von Teilchen, die durch merh als eine Zelle gehen?