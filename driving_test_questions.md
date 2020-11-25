1. Which of the following statements about HPC are true?
(select all the ones that apply) 
* Communications speed over the interconnect is unimportant because the processors themselves are so fast
* High Performance Computing is synonymous with parallel computing
* The processors used are always the most powerful, cutting edge designs available
* Computations run on multiple processor-cores at the same time


2. Leeds ARC4 uses which type of processor:
* AMD Opteron
* NVIDIA Kepler
* Intel Xeon Phi
* IBM Power7
* Intel Xeon (Ivy Bridge)


3. Jobs on ARC4 should be run from within which filesystem?
* Your home directory
* /PBS
* /nobackup
* /general


4. Which of the following are filesystems attached to ARC4:
(select all the ones that apply) 
* Home directories
* Work
* Nobackup
* Shared
* Research Data Storage
* Archive


5. ARC4 uses the "modules" environment to manage access to different software components. If you were interacting with the "castep" module, which of the following are valid module commands?
(select all the ones that apply) 
* module version castep
* module help castep
* module load castep
* module export castep
* module update castep


6. You want to share some files on ARC with someone else in your research group. Where could you put them so that the other user can easily copy or read them?
(select all the ones that apply) 
* /home/g01/shared/
* /work/g01/shared/
* /home/g01/g01/shared/
* /work/g01/g01/shared/



7. Which of the following tools would you generally use to open an interactive terminal on the HPC login nodes from your local computer?
* vi
* bash
* ssh
* Telnet
* rlogin


8. What term is used to describe the problem of some sub tasks taking substantially longer to complete than others?
* Task farm
* Load weighting
* Task stealing
* Load imbalance


9. Which of the following tools would you generally use to copy small amounts of data from your local system to ARCHER?
* scp
* ftp
* mv
* nano
* bash


10. Which of the following are transfer utilities suitable for copying very large amounts of data between a remote system and ARCHER? (select all that apply)
* GridFTP
* cp2k
* bbcp
* cp


11. You normally run computational code on your laptop or local computer but are now moving to Leeds HPC. You usually run some Python scripts to do post-processing and make nice graphs. Which of the following can you do on Leeds HPC? 
* Run code & post-processing
* Run code only
* Run post-processing only


12. You want to list all the loaded modules. Which command should you use?
* module avail
* module list
* module show
* module help


13. How would you replace the Intel compiler environment with the gnu compiler environment. 
* module replace intel gnu
* module swap intel gnu
* module swap compiler-intel compiler-gnu
* module swap gnu intel


14. You have been running an application on a local computer, and you now want to use ARCHER. The application uses the standard scientific libraries PETSc and LAPACK. Should you: 
* copy the application source code and compile using existing library modules on ARCHER.
* copy the application binary from your local computer to ARCHER, and run directly.
* copy the application and library source code to ARCHER, and compile.
* copy the application source code and library binary to ARCHER, and compile.


15. Put the following in the correct order in time as they occur for a simple batch job on Leeds HPC which makes a single call to "mpirun".
* the executable is broadcast to the compute nodes
* the job script is executed on the MOM nodes
* the user issues the "qsub" command
* PBS takes a copy of the user's job script
* resources are allocated for the job


16. You want to use an application on Leeds HPC that has a graphical user interface, or you simply want to plot some images using data stored on Leeds HPC and see these directly on screen without saving them and transferring the resulting files across to your own computer first. Is this possible? 
* No, you can only send and receive text commands to and from ARCHER using the terminal
* Yes, provided you login to ARCHER using the command ssh -X or ssh -Y, which enable forwarding of graphics to your own computer over the SSH connection
* It depends on whether you have enough kAUs left in your budget
* Yes, but it requires logging in to the special GUI-enabled login nodes


17. How many jobs can one user submit to the queuing system at one time?
* 4
* 8
* 16
* 32
* unlimited


18. Approximately how many (compute) cores are there on ARC4? 
* 100,000
* 500,000
* 10,000
* 7,000
* 1,000,000


19. What is the maximum memory available on any ARC4 compute node? 
* 8 GB
* 16 GB
* 64 GB
* 192 GB
* 768 GB


20. Why should the /home filesystem be used for critical data such as source code? 
(select all that apply)
* it is designed for very high performance
* it has a large (more than a petabyte) storage capacity
* it is backed up on a daily basis
* it is accessible from the compute nodes
* it has a lifetime longer than the ARCHER service


21. What command is used to delete a job that has been submitted on ARCHER? 
* skill
* rm
* qdel
* llcancel


22. What is the longest duration a job can run for on Leeds HPC?
* 12 hours
* 24 hours
* 48 hours
* 96 hours


23. Which of the following are correct statements about typical large-scale HPC systems such as Leeds HPC? 
(select all the ones that apply) 
* Users log on to the back-end compute nodes to run jobs
* The overall system is shared with many users
* Jobs are submitted via a batch scheduling system
* The system is typically accessed using GUI-based tools
* Resources are tightly monitored and controlled


24. Which parallel filesystem is used in /nobackup directory?
* The /nobackup directory does not use a parallel filesystem
* Lustre
* GPFS
* GFS


25. You want to use a module called "fftw". Which command should you use?
* module load fftw
* module put fftw
* module start fftw
* module add fftw


26. This is an excerpt from a job submission script.

#!/bin/bash --login
#$ -N tpls
#$ -l select=31
#$ -l h_rt=1:00:00

mpirun -n numproc myexecutable

-------------------------------------------------------------

What is the maximum value allowed for the number of processes <numproc> to allow the parallel job to run successfully? 
* 1
* 24
* 512
* 744
* 1024


27. How many cores are there in each ARC4 node? 
* 1
* 2
* 16
* 32
* 40


28. How can I contact to the Research Computing helpdesk? (select all that apply)
* Via The IT Servicedesk
* By email
* By post
* By phone









