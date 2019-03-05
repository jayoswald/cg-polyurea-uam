LAMMPS data file and input file for running united-atom model simulation


uam-8b120c.lammps:
LAMMPS data file of a polyurea system with 120 8-block chains.

in.lammps:
Input file for running UAM coarse-grained simulation.
The whole process in the input file is similar to the one in UAM paper, 
which takes approx 26 hours using 224 processors (Intel Sandybridge Xeon).

uam-8b120c-nvt.lammpstrj:
The resulted trajectory of super-atoms during NVT process.
Phase-segregated morphology can be visualized from trajectory dump file via VMD software.

If want to run a simulation starting with phase-segregated morphology, uncomment line:
"#read_dump      uam-8b120c-nvt.lammpstrj 0 x y z" in in.lammps.
