Table generated:
![[Pasted image 20220201113022.png|900]]
- Each hit simulation runs x muons per job
- Use TBrowser to view leaves
- Geant4 uses half lengths, ROOT uses full lengths for geometry
- Look at DUNE paper table
- Histogram
	- Third colour of any interesting isotopes
- Also have additional information with timing
	- `Time` in nano seconds
	- Divide into prompt and delayed
	- Anything within 20 micro seconds is considered prompt
- Geant4
	- EventAction -> Data saved to disc, have a look at details


## Quea
- #question What is the difference between logs and data?
	- logs are just print statments
- #question What does the Score mean when using TChain?
	- Just the name of the object
- #question How to draw the TPC detector volume using TCanvas -> https://root.cern.ch/doc/master/classTGeometry.html
	- Two options:
		- TGeoManager -> can load GDML file
		- Draw whole detector again using ROOT
- #question How to identify volume hit location in
	- VCode
- #question What are volume codes?
![[Pasted image 20220130225905.png|300]]
- These are the `VCode` in ROOT
- How to histogram
	- Pass string (Some commands) or  TCut object
	- `chScore->Draw("IonA")``