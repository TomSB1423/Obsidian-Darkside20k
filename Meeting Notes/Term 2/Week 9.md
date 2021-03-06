# Work Done
Writing the report
- Tried doubling the deadtime to see effect on counts per volume:
```
Buffers:
No: 181
Total Counts: 191335006
Total Production (yr): 6595484.522578421
Number of stable isotopes: 39
Number of unstable isotopes: 142

TPC Prompt:
No: 170
Total Counts: 79525683
Total Production (yr): 2741319.6483971043
Number of stable isotopes: 39
Number of unstable isotopes: 131

TPC Delayed:
No: 93
Total Counts: 18009353
Total Production (yr): 620798.1041020337
Number of stable isotopes: 39
Number of unstable isotopes: 54

TPC Prompt 2x:
No: 170
Total Counts: 81820621
Total Production (yr): 2820428.162702516
Number of stable isotopes: 39
Number of unstable isotopes: 131

TPC Delayed 2x:
No: 93
Total Counts: 15714415
Total Production (yr): 541689.5897966217
Number of stable isotopes: 39
Number of unstable isotopes: 54
```
- ![[Pasted image 20220301161344.png|500]]
- Didn't make any difference - > Same number of isotopes produced & counts did not change at all
- Started writing the report & making results tables


# Meeting
- Tried plotting energy distribution:
	- ![[Pasted image 20220302183913.png|500]]
- What is muangle
	- ![[Pasted image 20220302210513.png|500]]
- Found Be 4-8 and this ALPHA decays?! Is this expected?
- How much memory does the simulation output use -> so I can quote in report?
- What to do when decays like this?
	- ![[Pasted image 20220303201504.png|500]]
- Importance of electron recoils -> this is what I understand:
	- WIMPs cause mainly nuclear recoils in the range 30-200keV but also limited electron recoils in the range 4-50keV
	- Determine sensitivity of nuclear recoil searches as discrimination between NRecoil and ERecoil is not perfect
	- Neutrinos are much more likely to ERecoil than NRecoil so we discard all ERecoils? Or do we partially discard parts of the ERecoil spectra?
	- **Main question is does DarkSide specifically look for WIMP energy depositions in NRecoil or ERecoil or both?**
- Do q-values actually mean anything or is it just beta/gamma decay energy?
- What about energy deposition vs radioactive decay?
	- Lots of delayed so EDep can be a WIMP like event?
- No simulation of the outer 700t of UAr -> wouldn't this provide some shielding?
- Why is it just tritium that you are searching for? -> surely it is other isotopes too?
- Have you included the fiducial volumes?
	- Or can I just multiply all TPC volumes with a ratio
	- Don't need to
- What else to write


- Source of Be
	- Enormous energy photons but likely a neutron -> as can move around for longer distances and therefore generate a delayed
	- Neutrons "thermalize" as they diffuse
	- Neutrons have a 2ms cut
	- Alpha particles can actually give nuclear recoils
	- Others only mimic WIMP events at low energy

- Talk about electron recoils for low energy wimps
	- Beta decay important for background for electron recoils
	- Discrimination between electron and nuclear is hard at low energy
	- No S1 signal at low energy for ERecoil
	- Threshold for NR is 30keV
	- neutrino scattering