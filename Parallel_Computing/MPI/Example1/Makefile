#==========================================================
# Make file for pi_monte_carlo.f90
#==========================================================
F90CFLAGS   = -c -O2
F90COMPILER = mpif90
PRO         = pi_monte_carlo
OBJECTS     = $(PRO).o

${PRO}.x : $(OBJECTS)
	$(F90COMPILER) -o ${PRO}.x $(OBJECTS)

%.o : %.f90
	$(F90COMPILER) $(F90CFLAGS) $(<F)

clean : 
	rm *.o *.x
