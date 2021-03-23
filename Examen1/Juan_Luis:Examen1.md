1. Mention three differences in hardwer that exist between a normal pc and a high performance computer. 
	- The number of processors
	- The number of GPUs
	- The cooling systems

2. Mention two network technologies that are used in high performance computing and what are their main characteristics. main characteristics.
	- Infiniband -> Fiber optic connection -> Parallel computation with MPI
	- Ethernet -> Networking for equipment access

3. Explain what a flop is
	- Floating point operations per second	

4. Mention three supercomputing centers in Mexico
	- Kan Balam Cluster (1368 processors) -> DGSCA -UNAM
	- Cray XD1 (216 processors) -> National Supercomputing Center (CNS)
	- Cluster Mezquite (140 processors) -> Univ. of Sonora
	
5. Outline the steps to install the MPI library and explain the differences in the message handler. 

	- Identify the message handler:
		 - hyra -> Launch processes using daemons (for clusters).
		 - gfork -> All the processes on a node
	- Download the tar we are going to install
	- Read the manual identifying to install the handler we need, as well as the compilers. 
	- gunzip
	- tar xvf -> extract and show only the archives
	
	
	* It is recommended to empty the swap when compiling.
		- sudo su
		- swapoff -a
		- swapon -a

		**Exit root**
	- ./configure ->  _Check the documentation to set the flags you need_
		> ./configure --with-device=ch3 --disable-fortran
	- make

	- make install

	* If there are errors when compiling:
		> make clean
		<compile again> -> make	


References:
- https://administracion.cinvestav.mx/Portals/0/SiteDocs/SPlaneacion/CGSTIC/Publicaciones/Supercomputo.pdf?ver=2I3UmnsS5p3b9Qr0pCJaIQ%3d%3d
