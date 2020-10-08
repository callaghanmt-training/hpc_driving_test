Which of the following statements about HPC are true?

(select all the ones that apply) 
	Communications speed over the interconnect is unimportant because the processors themselves are so fast
	High Performance Computing is synonymous with parallel computing
	The processors used are always the most powerful, cutting edge designs available
	Computations run on multiple processor-cores at the same time


ARCHER uses which type of processor:
	AMD Opteron
	NVIDIA Kepler
	Intel Xeon Phi
	IBM Power7
	Intel Xeon (Ivy Bridge)


Jobs on ARCHER should be run from within which filesystem?
	/home
	/PBS
	/work
	/general


Which of the following are filesystems attached to ARCHER:
(select all the ones that apply) 
	Home
	Work
	Project
	Shared
	Research Data Facility (RDF)
	Archive


ARCHER uses the "modules" environment to manage access to different software components. If you were interacting with the "castep" module, which of the following are valid module commands?
(select all the ones that apply) 
	module version castep
	module help castep
	module load castep
	module export castep
	module update castep


You want to share some files on ARCHER with someone else in your research group. Where could you put them so that the other user can easily copy or read them, assuming your group is g01 
(select all the ones that apply) 
	/home/g01/shared/
	/work/g01/shared/
	/home/g01/g01/shared/
	/work/g01/g01/shared/



Which of the following tools would you generally use to open an interactive terminal on the ARCHER login nodes from your local computer?
	vi
	bash
	ssh
	Telnet
	rlogin


You have just logged in to ARCHER and you wish to run a parallel application. However, your application builds with gnu or intel compilers only; how should you ensure that the source code is compiled correctly? 

(select all the ones that apply) 
	use the module command to change the default programming environment
	alter the makefile so that the gnu or intel compiler is called explicitly
	alter the makefile so that it uses the generic compiler wrappers (cc, CC or ftn)
	compile on a local Linux system which has these compilers and copy the executable to ARCHER


You have been running an application on a local computer, and you now want to use ARCHER. The application uses the standard scientific libraries PETSc and LAPACK. Should you: 
	copy the application source code and compile using existing library modules on ARCHER.
	copy the application binary from your local computer to ARCHER, and run directly.
	copy the application and library source code to ARCHER, and compile.
	copy the application source code and library binary to ARCHER, and compile.


Put the following in the correct order in time as they occur for a
simple PBS batch job on ARCHER which makes a single call to "aprun".
    the executable is broadcast to the compute nodes
	the job script is executed on the MOM nodes
 	the user issues the "qsub" command
	PBS takes a copy of the user's job script
	resources are allocated for the job


You want to use an application on ARCHER that has a graphical user interface, or you simply want to plot some pretty pictures using data stored on ARCHER and see these directly on screen without saving them and transferring the resulting files across to your own computer first. Is this possible? 
	No, you can only send and receive text commands to and from ARCHER using the terminal
	Yes, provided you login to ARCHER using the command ssh -X or ssh -Y, which enable forwarding of graphics to your own computer over the SSH connection
	It depends on whether you have enough kAUs left in your budget
	Yes, but it requires logging in to the special GUI-enabled login nodes


How many jobs can one user submit to the queuing system at one time?
	4
	8
	16
	32


By default, how many MPI processes does aprun place on each node?
	1
	12
	24
	48


Approximately how many (compute) cores are there on ARCHER? 
	100,000
	500,000
	10,000
	5,000
	1,000,000


What is the maximum memory available on any ARCHER compute node? 
	8 GB
	16 GB
	64 GB
	128 GB
	512 GB


Why should the /home filesystem be used for critical data such as
source code? 
(select all that apply)
	it is designed for very high performance
	it has a large (more than a petabyte) storage capacity
	it is backed up on a daily basis
	it is accessible from the compute nodes
	it has a lifetime longer than the ARCHER service


What command is used to delete a job that has been submitted on ARCHER? 
	skill
	rm
	qdel
	llcancel


You normally run computational code on your laptop or local computer but are now moving to ARCHER. You usually run some Python scripts to do post-processing and make nice graphs. Which of the following can you do on ARCHER? 
	Run code & post-processing
	Run code only
	Run post-processing only


What is the longest duration a job can run for on ARCHER?
	12 hours
	24 hours
	48 hours
	96 hours


Which of the following are correct statements about typical large-scale HPC systems such as ARCHER? 

(select all the ones that apply) 
	Users log on to the back-end compute nodes to run jobs
	The overall system is shared with many users
	Jobs are submitted via a batch scheduling system
	The system is typically accessed using GUI-based tools
	Resources are tightly monitored and controlled


Which parallel filesystem is used in /work directory?
	The /work directory does not use a parallel filesystem
	Lustre
	GPFS
	GFS


You want to use a module called "fftw". 
Which command should you use?
	module load fftw
	module put fftw
	module start fftw
	module add fftw


This is an excerpt from a PBS job submission script.

#!/bin/bash --login
#PBS -N tpls
#PBS -l select=31
#PBS -l walltime=1:00:00
#PBS -A z01

cd $PBS_O_WORKDIR

aprun -n numproc myexecutable

-------------------------------------------------------------

What is the maximum value allowed for the number of processes <numproc> to allow the parallel job to run successfully? 
	1
	24
	512
	744
	1024


How many cores are there in each ARCHER node? 
	1
	2
	16
	24
	32


How can I contact to the ARCHER helpdesk? (select all the ones that apply)
	Via ARCHER SAFE
	By email
	By post
	By phone









