#TODO Complete

Inelastic scattering of a particle and a target.
Neutrons are the most likely candidate (highest cross-section) for recoil interactions as they are uncharged and therefore are unaffected by electrostatic attraction.


#TODO Sort this paragraph out below, still messy ⬇️
Can be detected by exploiting two signals → defined as prompt & delayed signals: 
#question - <u> Are prompt and delayed signals only produced by neutrons? Is there any inherent scintillation light produced in the muon collision, or is it just afterwards? </u>

#question - <u> Would assume S2 would always be produced whenever a muon enters the TPC even if no interaction as there will be ionization occurring? Couldn't you use this information to determine that this was a muon and not a WIMP?</u>
-   Prompt signal is produced during the ethermalization of the neutrons → neutrons loose energy by scattering off nuclei of the scintillator (mainly hydrogen), this normally produces a short signal w.r.t scattering on argon
-   Delayed signal is due to neutron capture, the thermalized neutron can capture on isotope in the scintillator e.g B-10 → This produces light regardless of the energy of the neutron
-   So there could be a delayed signal without a prompt signal
-   To identify this: ([[S1 & S2 Signals#^ede160]])
	-   A delayed veto window is opened in the LSV after each event in the TPC. If scintillation signal above certain threshold is detected in the LSV then this TPC event is discarded
	-   But there can be events that are accidentally discarded due to radioactive contamination in the LSV → probability of this is calculated to an acceptable level


# Methods of Recoil
## Nuclear
#### Via Neutrons:
Neutrons that enter the LAr TPC come from primarily 4 sources:
-   Radioactivity in outside environment suppressed by [[Veto]] shielding
-   Cosmogenic interactions due to muons → suppressed by [[Veto]] shielding
-   Spontaneous fission reactions → Usually release multiple neutrons and high energy gamma-rays which increase the probability of multiple interactions in either the TPC or the neutron [[Veto]]
-   (Alpha n) reactions in the detector materials → This comes from radioactive isotopes in the detector medium e.g U and Th decay chains. Planned on using a liquid scintillator doped with and isotope with high cross-section for thermal neutron capture. However there are safety concerns.
These sources of neutrons must be reduced.

## Electron
Very similar to nuclear recoil, however iinstead of a nucleus, and electron is hit.
-   Reduction methods successful in darkside-50
-   Reduced by material screening (assume this to be veto), analysis cutting and PSD to identify between nuclear vs electron recoils
-   Sources:
	-   Solar neutrino induced electron scatters
	-   Uranium and other daughter products
	-   Ar-39
	-   Kr-85


## Surface Recoils
Occurs when a radioisotope decays on the interior surface of the detector. This may eject an alpha particle towards the wall and recoil into the active argon volume producing a nuclear recoil signal.


## Notes
#SomethingToThinkAbout Can also be nuclear interactions with muons and the rock surrounding the experimental halls which produce neutrons and other particles that potentially give backgrounds in DarkSide-type detectors

[Explains the PSD](https://www.pnnl.gov/main/publications/external/technical_reports/PNNL-21609.pdf)
