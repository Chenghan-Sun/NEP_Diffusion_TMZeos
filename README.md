# Supplemental Information for the TM@Zeolites Diffusion Paper

In this repo, the following data and model details were included:

	- The final trained NEP-iter5 MLP model (nep5_full.txt file) for 10ns diffusion studies, transferability, and scalability testings.

	- The input file (nep.in file) consists of for hyper-parameters used for developing NEP-iter5 MLP model.

	- The job.out file (training progress and results) of NEP-iter5 MLP model.

	- All the test sets (.db files) available in the testset-dbs-from-NEP-models folder, with:
		- Folder TMZeos-scalability has four ASE databases  (please refer this [link](https://wiki.fysik.dtu.dk/ase/ase/db/db.html#a-database-for-atoms) for using ASE.db)：
			- iter4_spe_from_nep4_200dumped_BEA.db: uniformed sampled 200 configurations from 200ps adaptive metadynamics for 3/6/9Au@BEA systems. 
			- iter4_spe_from_nep4_200dumped_CHA.db: uniformed sampled 200 configurations from 200ps adaptive metadynamics for 3/6/9Au@CHA systems.
			- iter4_spe_from_nep4_200dumped_MFI.db: uniformed sampled 200 configurations from 200ps adaptive metadynamics for 3/6/9Au@MFI systems.
			- iter4_spe_from_nep4_500dumped_RHO.db: uniformed sampled 500 configurations from 200ps adaptive metadynamics for 3/6/9Au@RHO systems (we further subsampled 200 trajs for the plot for consistency).
		- Folder Temp-transferability has four ASE databases:
			- iter5_spe_from_nep5_task2_300K_LTA.db: uniformed sampled 200 configurations from 1ns adaptive metadynamics under 300K for 3/6/9Au@LTA systems.
			- iter5_spe_from_nep5_task2_500K_LTA.db: uniformed sampled 200 configurations from 1ns adaptive metadynamics under 500K for 3/6/9Au@LTA systems.
			- iter5_spe_from_nep5_task2_700K_LTA.db: uniformed sampled 200 configurations from 1ns adaptive metadynamics under 700K for 3/6/9Au@LTA systems.
			- iter5_spe_from_nep5_task2_1000K_LTA.db: uniformed sampled 200 configurations from 1ns adaptive metadynamics under 1000K for 6/9Au@LTA systems.
		- Folder 10ns-metaD has only one  ASE databases:
			- iter5_spe_from_nep5_task3_10ns_LTA.db: uniformed sampled 400 configurations from 10ns adaptive metadynamics under 300K for 3/6Au@LTA systems for diffusion studies. 
	- The INCAR file for DFT single point calculations. 
	- PLUMED input files for both adaptive / well-tempered metadynamics (with reweighting) simulations.
