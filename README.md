# PCC-module-stability
There are two ls.dat files, new and old veto files consisting of run number, lumi section and pixel cluster count data

We need to divide new pixel cluster count (third column in ls_new.dat) by old pixel cluster count (third column in ls_old.dat)

While dividing, we need to make sure that we are dividing counts corresponding to same run number and lumi section in both the files.

Don't divide if count in ls_old.dat file is equal to zero.

Output of comparelsdotdat_express.C code is shown in c1.png image
