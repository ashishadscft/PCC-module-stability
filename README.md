# PCC-module-stability
There are two ls.dat files, new and old ls files consisting of run number, lumi section and pixel cluster count data

We need to divide new pixel cluster count (third column in ls_new.dat) by old pixel cluster count (third column in ls_old.dat)

Before dividing, remove all points with count <=3*10^3 as shown in compare_lsdotdat_Run2018A_old_new.png image

While dividing, we need to make sure that we are dividing counts corresponding to same run number and lumi section in both the files.

Don't divide if count in ls_old.dat file is equal to zero.

Output of the ratio of counts using comparelsdotdat_express.C code is shown in compare_lsdotdat_hist_Run2018A_newveto_ratio.png image. But probably, in this graph, division is not done by considering same lumi section corresponding to same run number.
