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
			- Capture and stopping#
		- Electromagnetic Component
		- Decay Component
		- Neutron tracking cut


# Results
- Intro
- Table
	- Prompt in TPC
	- Delayed in TPC
	- Buffers
- Compare models
	- All agree within factor 2 for all isotopes $A<21$ but then differ when looking at higher mass 
	- Can be confident that muons create lots of isotopes and some may be heavier that argon itself
	- uncertain about how exotic heavy though
- Found no Tritium anywhere
  - Tritium physics might not be included in geant4 as you need to build the material yourself
  - By default tritium does not decay
  - Or perhaps alternatively 
- No Isomeric transition for any decay -> no high energy gamma rays released anywhere
  - But could it just be possible that an ion is created and recombination creates a gamma ray?
  - Does this mean nothing to worry about in the outer buffer?
- By using 3 volumes and ignoring all prompt events can excluded ~84.11% of events ($1-(27.7\% * 57.2\%)$)
  - Delayed vs prompt split
    - ![[Pasted image 20220208184123.png|400]]
  - Total counts pretty much split into thirds over 3 different volumes:
  - ![[Pasted image 20220208184210.png|400]]

- Look at DUNE
- Show table & comment on relative abundances
	- Only highest yields
- muon spallation caused heavier isotopes to form
- Analysis of Background rejection
	- Prompt doesn't mean anything
	- delayed
	- percentage rejected

### Tritium production
- No tritium produced
	- Insight into xenon1 experiment - might not be from muons
	- So extra simulations run with different physics models

# Conclusions
