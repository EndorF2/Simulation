# Simulation
ENDORF2 simulation program for single crystal and disordered samples
The program is based on theory presented in [1, 2] for the simulation of single crystal and ‘powder’ ENDOR
spectra. It was written with the purpose of analyzing spectra of free radicals for a general case when the nuclear
quadrupole (nqc) and hyperfine (hfc) couplings of a nucleus may be of comparable magnitude.
A general theory to calculate ENDOR spectra of S=½ systems was employed under the assumption that the
electron Zeeman interaction is dominating. No restrictions were made on the relative magnitudes of the hfc nuclear
Zeeman and nqc splittings, the latter for nuclei with I>½.
The code is written in Fortran77 except for a few lines to read the computer clock (subroutine gettim available in
Microsoft Fortran Powerstation). Diagonalisation of the Hamiltonian Hi’ can be performed numerically for any
nuclear spin in the range ½ <= I <= 9/2. An analytic treatment available for nuclei with I=1/2, 1, and 3/2 [7] is ca 30 %
faster.  Any comments or suggestions on this version may be sent to:
Roland Erickson, Sweden, E-mail:roland.erickson@comhem.se
Anders Lund Linköping University, Department of Physics, Chemistry and Biology, Linköping University, Husett, S-581 83 Linköping,
Sweden, Email: anders.lund@liu.se

The program is also available on a homepage of Linköping University, https://old.liu.se/simarc/downloads?l=en, where other EPR simulation programs are also available for download.

Example input files for ENDORF2 simulation of powder ENDOR spectra of free radicals, including biphenyl radical cation, 14NO-ligated ferrocytochrome c heme a3 and irradiated hippuric acid are included in the ENDORF2 packages on the repository.

For comparative purposes input datafiles for powder simulation with exact diagonalisation using the externally available matlab programme Easyspin [https://www.easyspin.org] are also available, together with simulation results. These include the biphenyl and naphthalene radical cations, 14NO-ligated ferrocytochrome c heme a3 and irradiated hippuric acid. 

References

1. Erickson R (1995) Electron Magnetic Resonance of Free Radicals. Theoretical and Experimental EPR,
ENDOR and ESEEM Studies of Radicals in Single Crystal and Disordered Solids, Linköping Studies in
Science and Technology, PhD Thesis No 391, ISBN 91-7871-582-2, Linköping, Sweden
2. Erickson R (1996) Simulation of ENDOR spectra of radicals with anisotropic hyperfine and nuclear
quadrupolar couplings in disordered solids. Chem Phys 202:263-275
3. Erickson R, Lund A, Lindgren M (1995) Analysis of powder EPR and ENDOR spectra of the biphenyl
radical cation on H-ZSM-5 zeolite, silica gel and in CFCl3 matrix Chem Phys 193:89-99
4. Erickson R, Benetis NP, Lund A, Lindgren M, (1997) Radical cation of naphthalene on H-ZSM-5 zeolite
and in CFCl3 matrix. A theoretical and experimental EPR, ENDOR, and ESEEM study. J Phys Chem A
101:2390 –2396
5. Lund A, Erickson R (1998) EPR and ENDOR simulations for disordered systems: The balance between
efficiency and accuracy. Acta Chem Scand 52:261–274
6. Erickson R, Lund A (2014) Applications of EPR and ENDOR Spectrum Simulations in Radiation
Research. In Lund A, Shiotani M (eds) Applications of EPR in Radiation Research. Springer
7. Erickson R, Lund A (1991) Analytical Expressions of Magnetic Energies and Wavefunctions of
Paramagnetic Systems with S=1/2 and I=1 or I=3/2. J Magn Reson 92:146-151
