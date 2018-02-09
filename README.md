# LINPACK
The original (1000x1000 double precision) LINPACK benchmark, with bugfixes, from

http://www.netlib.org/benchmark/1000d

It has been altered slightly to use cpu_time(t) instead of expecting seconds() to be defined.

Build something like this (you may wish to add some compiler flags such as -O2):

   gfortran -W -Wall 1000d.f -o linpack-benchmark

And run:

    $ ./linpack-benchmark 
   Please send the results of this run to:
  
   Jack J. Dongarra
   Computer Science Department
   University of Tennessee
   Knoxville, Tennessee 37996-1300
  
   Fax: 615-974-8296
  
   Internet: dongarra@cs.utk.edu
  
       norm. resid      resid           machep         x(1)          x(n)
    6.49150133E+00  7.20701276E-13  2.22044605E-16  1.00000000E+00  1.00000000E+00
  
  
      times are reported for matrices of order  1000
        factor     solve      total     mflops       unit      ratio
   times for array with leading dimension of1001
    1.024E+00  4.000E-03  1.028E+00  6.505E+02  3.075E-03  1.836E+01
    end of tests -- this version dated 10/12/92
 

