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


## Questions
- What is the difference between logs and data?
	- logs are just print statements
- What does the Score mean when using TChain?
	- Just the name of the object
- How to draw the TPC detector volume using TCanvas -> https://root.cern.ch/doc/master/classTGeometry.html
	- Two options:
		- TGeoManager -> can load GDML file
		- Draw whole detector again using ROOT
- How to identify volume hit location in
	- VCode
- What are volume codes?
	- These are the `VCode` in ROOT
![[Pasted image 20220130225905.png|300]]
- How to histogram
	- Pass string (Some commands) or  TCut object
	- `chScore->Draw("IonA")`


Into to ROOT: [[https://www.phenix.bnl.gov/phenix/WWW/publish/tlthomas/GettingStarted.htm]]

## TODO:
- [ ] Look at DUNE paper - read all of it again
	- [ ] Make list of main points covered in paper
- [ ] Get detector location output working
	- [ ] Investigate different products dependent on location
- [ ] Play around with TBrowser & Histograms
- [ ] Get detector yield per muon & per day