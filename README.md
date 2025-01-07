# Amber_salt_ions_concentration_calculater

This code calculates the number of ions to be added to an amber system based on the salt concentration you want in your system. 

Example: Consider the example shown on the amber official page Link: https://ambermd.org/tutorials/basic/tutorial8/index.php you want to calculate the number of ions for this system to match physiological conditions. 

When you run this code, it will ask for volume in Å3. Enter the value as 208141.839 Å3 and set the salt concentration to 0.150mol/l. It will calculate the number of NA and Cl ions.

Note: These ions will be added to the number of ions you add to neutralise the system. 

# Amber_salt_ions_concentration_calculater(SPLIT_method) - Recommended one 

This method is based on Machado et al., 2020 (J. Chem. Theory Comput. 2020, 16, 3, 1367–1372) All credits go to the original authors of the paper.

Link to the original paper: https://doi.org/10.1021/acs.jctc.9b00953

Example: Consider the example shown on the official website of Amber Link: http://archive.ambermd.org/202002/0194.html which includes ion concentration calculation for Lysozyme  system (PDB: 2VB1), Q = +8e, Water box 12Å => Nw ~ 7000 molecules, [NaCl]=0.15M

When you run this code, it will ask for the number of water molecules. Please enter the value as 7000 (as given above; it can be obtained from the leap.log file) and set the salt concentration to 0.150mol/l. The code also asks for the total charge on the solute (it can be obtained from the leap.log file). It will calculate the number of NA and Cl ions as 15 and 23, respectively.

If the charge on your solute is not an integer, please round it off first.

Note: These ions include those required to neutralise the system so there is no need to add extra ions apart from these. 
