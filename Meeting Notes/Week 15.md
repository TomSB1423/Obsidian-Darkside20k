- SCRTP account
- Yorck will tell how to access output files
- Simulation output to ROOT
- ROOT is C++ / python though not sure for python
- Electron recoil for low energy WIMPS
- Mainly looking for beta decay as alpha decay not likey as isotopes have low mass
- Then once identified the main isotopes to look for simulate again with same geometry however now with that isotope distributed as expected and see is significant to WIMP detection
- batch selection: slorm? (SCRTP wiki)
	- sq command - lists every schedule on all command


Recommends sticking with C++

Can find simulation outputs at `/storage/epp2/phsdaq/MuOnArgon/`
- `batch` contains an example ROOT script

In order to use root:
- Load modules
	- `module use /warwick/epp/modules`
	- `module load linuxbrew/supernemo`
- Start ROOT:
	- `root`
- Load the Script:
	- `.L analyseRootOutput`
- Call methods:
- `fullSummary("fnames.txt")`