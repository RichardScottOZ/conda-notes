# conda-notes
Notes of relevance to working with the Anaconda python distribution

# Distributions
- Full Anaconda
- Miniconda [my preference]
- Micromamba [minimalist shell install useful for headless machine install of a minimal set of packages]
	- https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html
		- Note that of course the installation url could change if you are automating installaions from the above
	- For example into an AWS EC2 Deep Learning AMI
- Mamba : the libmamba solver in the latest conda seems to be working well so far
	
# Environments
- Activation scripts are different between Linux and Windows
- conda-pack is useful to transfer a working environment from one machine to another
	- It must be created on the same operating system as you are going to use it on as it is packaging necessary files/binaries
		- Ubuntu -> Ubuntu
		- Windows Server 2016 -> Windows Server 2016
		
	- There are other things you can do than an install to a default home directory
	- Need example
	- References
		- https://gist.github.com/pmbaumgartner/2626ce24adb7f4030c0075d2b35dda32 -> Windows conda pack notes
		- https://stackoverflow.com/questions/59392191/import-existing-conda-environment-from-network-location
		
	
	```
	C:\Users\rscott>robocopy.exe C:\Users\rscott\Downloads\pangeo \\boringnetworkfolder\pangeo /E . /W:1 /R:1 /NFL /MT:64
	```