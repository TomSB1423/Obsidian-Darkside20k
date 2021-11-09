# Signals in the Detector
Categorized into two groups:
-   S1 → Scintillation signal
	-   Used for [[Energy Determination]] and for [[PSD]]	
	-   In principle more energy going into S1 than S2 as takes less energy to produce S1
		-   This is due to... #TODO
-   S2 → Ionization signal
	-   Used for energy and 3D position determination
	-   Proportional to the ionization charge
	-   Vertical coordinate measured from the drift time between S1 (start point) and S2 (end point, where electrons are detected)
	-   The horizontal coordinate measured from the light pattern on the top photosensors
		-   The TPC has a PCB board with holes in it which detect the angle at which the electrons have come in by
	-   S1 + S2 = constant → due to conservation of energy
	-   Introducing a stronger electric field means that there will be more charge produced → this would increase the S2 signal
		-   As electrons cant recombine with argon after they are ionized and so get carried away with the electric field
	-   Fiducialization that is typical of dual-phase detectors is not  possible without an S2 signal #question - <u>Why is this?</u>
		
Using both S1 & S2 means that a very good resolution can be obtained

#TODO talk about background rejection, include Cherenkov light and time rejection