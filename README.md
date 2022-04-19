# PCC-module-stability
There are two ls.dat files, new and old veto files consisting of run, lumi section and pixel cluster count data
We need to divide new pixel cluster count (third column in ls_new.dat) from old pixel cluster count (third column in ls_old.dat)
while dividing, we need to make sure that we are dividing counts corresponding to same run number and lumi section in both the files.
Don't divide if count in ls_old.dat file is equal to zero.
