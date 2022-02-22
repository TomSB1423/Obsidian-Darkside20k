## Work Done

### Tables generated:

- Unstable isotopes sorted by counts in all detector volumes
- Heavy instable isotopes
- Unstable isotopes sorted by half-life
- Highest production yields
- Delayed and prompt TPC sorted by Q-value

- Complete isotope volume + counts
- Prompt TPC - not too much an issue as are ignored due to deadtime
  - Prompt TPC counts
- Look for beta decay + excess yields
  - Delayed TPC counts
- Look for high energy gamma in outer buffers:
  - Buffers (prompt + delayed)

[[WC-Format.pdf]]

### Conclusions

- Found no Tritium anywhere! -> speak to Yorck about this
  - Other physics models -> currently use Shielding model
- No Isomeric transition for any decay -> no high energy gamma rays released anywhere
  - But could it just be possible that an ion is created and recombination creates a gamma ray?
  - Does this mean nothing to worry about in the outer buffer?
- By using 3 volumes and ignoring all prompt events can excluded ~84.11% of events ($1-(27.7\% * 57.2\%)$)
  - Delayed vs prompt split
    - ![[Pasted image 20220208184123.png|400]]
  - Total counts pretty much split into thirds over 3 different volumes:
  - ![[Pasted image 20220208184210.png|400]]
- Buffers high q-values (looking for gamma rays):
  - ![[Pasted image 20220216144940.png|900]]
    - Are these high or not?
    - Found that energies above ~200keV are unlikely to be in any WIMP model and can be excluded?
    -
- Looking for excess yields

  - Lots of potassium, 10% production yield -> but this is stable
  - Lots of Ar-39 produced
  - Might be worth looking at [this](https://arxiv.org/ftp/arxiv/papers/1712/1712.04399.pdf) paper

- Nice [dissertation](https://uh-ir.tdl.org/bitstream/handle/10657/7989/POUDEL-DISSERTATION-2020.pdf?sequence=1&isAllowed=y) on DarkSide
- Found VERY GOOD [this article](https://www.annualreviews.org/doi/10.1146/annurev.nucl.54.070103.181248) for muon backgrounds: - Also has some info about muon flux
  ![[Pasted image 20220221141637.png]]

- $1*10^{16} ns$ is about the upper limit in half life for anything reasonable
- Could think about plotting theoretical decay spectra of different important isotopes
-

# Meeting

- What would be a good way to narrow down the tables, production yields?
  - How to classify production yield? Is it the total volume, or just TPC?
- Organise a time to go through interim report
- Why do we ignore neutrino background?


#### Suggestions
- Look for activity -> look this formula up
	- Also production yield per year
- Work out how many years the simulation was using 1x10^7 muons and their flux
	- I should also hand over the muon flux underground at Gran Sasso: (3.477+-0.002)10^-4 m^-2 s^-1 GERDA collaboration, Astropart. Phys. 84 (2016) 29 The simulation muon source area is a circle with radius 10 m, i.e. 314.159 m^2 area, giving you 3.447e6 muons per year, our 1e8 simulated hence correspond to 29.01 years.
- less than 1 event per year on nuclear recoils
- Select isotopes for next week
- A further simulation can select dangerous isotopes, evenly distribute them over the TPC and then run a simulation for gamma rays writing their energy deposition to disk and seeing which contribute to WIMP signals
- Look up low background errors
