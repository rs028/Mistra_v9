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

1. Install __KPP-Mistra__. Please refer to the `README.md` file in the
[KPP-Mistra repository](https://github.com/MistraModel/KPP-Mistra) for
instructions.

1. Install a Fortran compiler (preferably __ifort__, alternatively
__gfortran__) and the __netcdf__ development libraries.

1. Check that the C shell (`csh`) is installed on your system, then generate
the mechanism files: in `src/mech/`, run `make`.

1. Check that netcdf libraries are installed on your system (`locate
netcdf.inc`). If not, install the package `libnetcdff-dev`. Edit the
`Makefile` (in the main directory), set the correct path to the netcdf
libraries and include file. Depending on netcdf distribution, use
`-lnetcdf` or `-lnetcdf -lnetcdff`.

1. Compile the code using `make`.

1. In the `param/param_...` file, set the appropriate path to Mistra
input files. It is advised to use a directory that will not be
duplicated for each version the user will run, but choose a generic
directory instead. Set the appropriate path to the parent output
directory, to the executable, and set the namelist to be used. Run
the `param_...` file to run the model.

For more detailed information see the pdf file in the `doc/` directory.
