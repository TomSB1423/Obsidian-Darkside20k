- Writing our own ROOT files
	- Identify isotopes
	- Which are stable
	- Classify into long lived and short lived ~ look at experiment definition
	- Also isotopes that decay after really long times are not interesting
	- Look at production yields per muon
	- Could normalise to the mass of the volume -> per kg of argon, but not too useful as this is constant
		- Could relate to Argo experiment

- Root TChain inherits from TTree
	- Look up specific examples -> best way of learning
	- Root also has a visual method -> `StartViewer()`
	- Though will want to write about code rather than viewer in the report

- Simulations so far are purely production simulations
	- Write ions produced from muon decays to disk
	- No tracking of the history
	- radioactive decay switched on
- Time information is useful in determining if dangerous or not
