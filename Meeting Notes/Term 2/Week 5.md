## Work Done
### Summary
1. Played around with histograms, but wasn't really successful in making them work
	- Found this [better site](https://root.cern/doc/master/classTTree.html#ac4016b174665a086fe16695aad3356e2) & [site](https://root.cern/doc/master/classROOT_1_1RDataFrame.html) for intro to histograms
	- Trying to work out how to draw two plots on the same histogram
		- ![[Pasted image 20220208180105.png|500]]
2. Tried opening GDML file however got segmentation fault
	- https://root-forum.cern.ch/t/error-when-visualizing-geometry-in-gdml-format-with-tgeomanager/19580
	- However tried again and got only a cube:
		- ![[Pasted image 20220208145423.png|900]]


3. Separated events into prompt and delayed and analysed ratio between the two
	- How is there scandium as a delayed event inside the TPC?
		- ![[Pasted image 20220208182705.png|900]]
		- Only one count in total for Sc? However lots of calcium and potassium
		- #question Only really three possibilities?
			- $^{42}$K + alpha -> Sc
			- $^{42}$Ca + Tritium -> Sc 
			- $^{43}$Ca + Deuterium -> Sc
			- But looking at the production yields, it seems like potassium + alpha is most likely as much more made
			- #question However how is this potassium even made in the first place?
		- Loads made as delayed rather than prompt
			- ![[Pasted image 20220208184123.png|400]]
			- Total counts pretty much split into thirds over 3 different volumes:
				- ![[Pasted image 20220208184210.png|400]]
	- By using 3 volumes and ignoring all prompt events can excluded ~84.11% of events ($1-(27.7\% * 57.2\%)$)


## Meeting
- Can we go over why both electron and nuclear recoils are important?
- Point 3. about scandium and potassium
- TGeoManager
	- Are different "modes" to view the geometry
	- Manipulate world volume with a mouse
	- Can draw wireframe
	- only need to draw the sensitive volume to hits


T vector of mass numbers 


- New trajectory is factor 10 less (10^7) than for before
	- End product is always an ion
	- Start is a muon
	- Fixed eventId is the same for every row
	- Draw points for interaction locations and draw a line
	- 