# Abstract
- Overview
- Look at DUNE paper
- Comment on background free experiment

# Introduction
#### Evidence for Dark Matter
- Expand on gravitational lensing + galactic rotation curves
- Maybe subsection on both?

#### Dark Matter Candidates
- Ask Yorck if this is a succinct description of dark matter, or need to expand more on each candidate?

### Detection Methods
- Emphasise low background physics
- WIMPs are anything that is unknown at this point?
- Link to detectors and state how they use background mitigation techniques

#### Background sources
- Ask Yorck if these are really the only two non-reducible sources of dark matter experiments
- Necessity of background suppression

#### WIMP Signatures
- Are there any more signatures?

### Sensitivity Prospects

### DarkSide Collaboration
- Just expand on each section

# Methodology
- **Simulation Process:**
	- Use of Geant4
	- Geometry production
		- GDML file
		- ROOT
	- Muon simulation -> $10^8$ muons, define flux using $10m^2$ 
		- I should also hand over the muon flux underground at Gran Sasso: (3.477+-0.002)10^-4 m^-2 s^-1 GERDA collaboration, Astropart. Phys. 84 (2016) 29 The simulation muon source area is a circle with radius 10 m, i.e. 314.159 m^2 area, giving you 3.447e6 muons per year, our 1e8 simulated hence correspond to 29.01 years.
		- Using shielding model
		- Addition physics list simulation in case of different products
		- Further trajectory simulation -> $10^7$ muons
- **Analysis**:
	- Open data in python
	- Added decay modes to each isotope
	- Calculate production per year
	- Separate into stable and unstable
	- Filter by realistic halflife -> all greater than 1 year excluded
	- Used API to identify isotopes that have an intensity > 0.5 with a mean beta decay energy between 0-200 keV
	- Looked for location specific decays:
		- Buffer -> any beta/gamma
		- TPC
			- Prompt -> ignored unless half life greater than dead time
			
	
- Comparison to DUNE
- Use parts of interim report + DUNE paper
- Geant4 simulation generates ROOT output
- Analysed using root and python
- Subsequent geant4 simulations were run with different physics models
	- Shielding -> Shielding is recommended for applications for neutron transport.
		- Hadronic Component
			- Inelastic models
			- Inelastic cross sections
			- Elastic models
			- Elastic cross sections
			- Capture and stopping
		- Electromagnetic Component
		- Decay Component
	- FTFP_BERT is recommended for collider physics applications. Differs from shielding in elastic cross sections and differing decay components implemented. FTFP also integrates a neutron tracking cut.
		- Hadronic Component
			- Inelastic models
			- Inelastic cross sections
			- Elastic models
			- Elastic cross sections
			- Capture and stopping
		- Electromagnetic Component
		- Decay Component
		- Neutron tracking cut


# Results
- **Plan:**
- Introduce muon spallation and a summary of all isotopes produced
- ![[Pasted image 20220304130352.png|300]]
- Location specifics of where isotopes are produced
- ![[Pasted image 20220208184210.png|300]]
-  ![[Pasted image 20220208184123.png|300]]
	- Buffers -> gamma
	- Rest of detector -> Not really an issue
	- **Table Image**
	- TPC
		- Prompt -> any with long half life
		- Delayed -> beta and gamma
			- Comment on no tritium
			- Tried doubling deadtime -> didnt do anything
	- ![[Pasted image 20220304130914.png|300]]
	- Compare models

- Quite good: https://www.sheffield.ac.uk/polopoly_fs/1.426340!/file/PHY326-2014-15-18.pdf
- Intro
- Table
	- Prompt in TPC
	- Delayed in TPC
	- Buffers
- Compare models
	- All agree within factor 2 for all isotopes $A<21$ but then differ when looking at higher mass 
	- Can be confident that muons create lots of isotopes and some may be heavier that argon itself
	- uncertain about how exotic heavy though
- Found tritium produced
- Gamma rays are going to be produced in buffer
	- But need to run another genat4 simulation
	- Would think this would introduce more false detections
- By using 3 volumes and ignoring all prompt events can excluded ~84.11% of events ($1-(27.7\% * 57.2\%)$)
  - Delayed vs prompt split
    - ![[Pasted image 20220208184123.png|400]]
  - Total counts pretty much split into thirds over 3 different volumes:
  - ![[Pasted image 20220208184210.png|400]]

- Look at DUNE
- Analysis of Background rejection
	- Prompt doesn't mean anything
	- delayed
	- percentage rejected
- Tried doubling deadtime -> didnt do anything
- "Calculations checked against those in Ref. [17] predict 1.6 events from this source in the full DarkSide-20k exposure." From: [[Darkside-20k first.pdf]]

# Conclusions
****