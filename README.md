            _     _             
           (_)   | |            
  _ __ ___  _ ___| |_ _ __ __ _ 
 | '_ ` _ \| / __| __| '__/ _` |
 | | | | | | \__ \ |_| | | (_| |
 |_| |_| |_|_|___/\__|_|  \__,_|
                                
                                

---

__Mistra__ is 

For the license see

For Credits see


HOW TO RUN MISTRA -- in a nutshell:
-----------------------------------

1) Install KPP. Please refer to the README file in the kpp/ directory for instructions

2) Install a Fortran compiler (preferably ifort, alternatively gfortran) and the netcdf libraries

---

3) Check that C shell (csh) is installed on your system, then generate the mechanism files: in src/mech, run make

4) Check that netcdf libraries are installed on your system (locate netcdf.inc). If not, install the package libnetcdff-dev
Edit the Makefile (in main directory), set the correct path to the netcdf libraries and include file. Depending on netcdf distribution, use "-lnetcdf" or "-lnetcdf -lnetcdff".

5) Compile the code using "make".

6) In the param/param_... file, set the appropriate path to Mistra input files. It is advised to use a directory that will not be duplicated for each version the user will run, but choose a generic directory instead.
Set the appropriate path to parent output directory, to the executable, and set the namelist to be used.
Run the param_... file to run the model.

For more detailed information see the pdf file in the doc/ directory
