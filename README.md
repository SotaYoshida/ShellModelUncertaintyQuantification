# ShellModelUncertaintyQuantification
Shell-model results of p-shell nuclei with uncertainty quantification

This is the repository to provide updated version of the results discussed in the following article:  
Uncertainty quantification in the nuclear shell model  
Sota Yoshida, Noritaka Shimizu, Tomoaki Togashi, Takaharu Otsuka  
DOI: 10.1103/PhysRevC.98.061301  

**New 0p-shell interaction: z_mass.int**  
This is the latest 0p-shell interaction for the 0p-shell in isospin-formalism.  This is optimized to the "original" 33 data set in the pioneering work by Cohen and Kurath: S. Cohen and D. Kurath, Nucl. Phys. 73, 1 (1965).  

The integers 3 and 4 represent the p1/3 and p3/2 orbits respectively.  
The interaction in the input format for KSHELL is also available. -> [z_mass.snt]  

**pshell_data.txt**

Experimental and calculated results are summarized in [pshell_data.csv]

Jnum: total angular momentum  
JTN: The "specifier" of the states. For example, (JTN=2+0,3) means the third lowest Jpi=2+ and T=0 state.  
Eexp: Experimental energy eigenvalues from ENSDF (Note: This can be outdated)  
ExExp: Experimental excitation energies of the states 
CKE(CKEx): Calculated energy eigenvalues (excitation energies) using the Cohen Kurath interaction (CKtb1 in our paper)    
EMAP(ExMAP): Results with the z-mass interection  
LA: mean values energy eigenvalues with 50,000 LA (Laplace Approximation) samples.  
LAsig: one standard deviaiton of the LA result  
Eim4(Exim4): Results with VS-IMSRG 500/400  
Eim5(Exim5): Results with VS-IMSRG 500/500  
infit: whether or not used in parameter fitting  

Remarks on LA families:  
"(1)" means that the Hessian matrix is evaluated only with the first derivative terms  
"ex" is used to abbreviate "excitation energy"  

For VS-IMSRG results (Eim4&Eim5):  
The interactions are opened by Ragnar Stroberg on GihHub:https://github.com/ragnarstroberg/PRL118032502

See the following paper for more details:  
S.R. Stroberg, A. Calci, H. Hergert, J.D. Holt, S.K. Bogner, R. Roth, and A. Schwenk,  PRL 118, 302502 (2017), arxiv 1607.03229  
