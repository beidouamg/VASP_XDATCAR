# VASP_XDATCAR
A python class for parsing VASP XDATCAR from molecular dynamics.

The XDATCAR file contains the trajectory during a molecular dynamics run, i.e.
the positions of all the atoms at each time step.  From this information, we may
calculate the following physical quantity

1. the time-dependent temperature of the system
2. Velocity Autocorrelation Function (VAF) and Phonon Density of States
3. Pair Correlation Function (PCF)

NOTES

    Set NBLOCK = 1 in the INCAR so that all the configuration in the MD run is
    wrtten to XDATCAR.

    The element mass (POMASS) and the MD time step (POTIM) is read from OUTCAR.
