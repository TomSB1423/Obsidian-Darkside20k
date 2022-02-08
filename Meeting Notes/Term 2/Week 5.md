## Work Done
### Summary
1. - Tried opening GDML file however got segmentation fault
	- https://root-forum.cern.ch/t/error-when-visualizing-geometry-in-gdml-format-with-tgeomanager/19580
	- However tried again and got only a cube:
	- ![[Pasted image 20220208145423.png|900]]
- #question Can we go over why both electron and nuclear recoils are important?


- Found this [better site](https://root.cern/doc/master/classTTree.html#ac4016b174665a086fe16695aad3356e2) & [site](https://root.cern/doc/master/classROOT_1_1RDataFrame.html) for intro to histograms
- Trying to work out how to draw two plots on the same histogram
	- ![[Pasted image 20220208180105.png|500]]
- How is there scandium as a delayed event inside the TPC?
	- ![[Pasted image 20220208182705.png|900]]
		- Only one count in total though?
		- However lots of calcium and potassium
		- #question Only really three possibilities?
			- $^{42}$K + alpha -> Sc
			- $^{42}$Ca + Tritium -> Sc 
			- $^{43}$Ca + Deuterium -> Sc
			- But looking at the production yields, it seems like potassium + alpha is most likely as much more made
			- #question However how is this potassium even made in the first place?
	- Loads made as delayed rather than prompt
		- ![[Pasted image 20220208184123.png|400]]
		- Counts pretty much split into thirds over 3 different volumes:
			- ![[Pasted image 20220208184210.png|400]]
		- 