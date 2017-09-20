Set-up issues:

1-This version is compatible with ViennaRNA-2.3.1, be sure the used version is above.
2-To use canvas please please set-up pyx as follow: 
-Download pyx-0.12.1.tar.gz 
-cd directory_containing_setup.py
-pip install .
-python setup.py install
3- VArna version VARNAv3-93.jar should be in the working repository.

How to use Rnastruct in our lab:

First go to the working directory :
	cd asaaidi/RNAstruct
to Launch the program:
	python Rnastruct.py 

For the configuration please us ethe file: RNAstruct.Config

*******************************************Input files:*************************

-fasta_Shape: contains constraint files with shape reactivity file. for each condition you should have two files: condition.fa and conditionShape.txt
where condition.fa: is a fasta file (sequence) with the identifier >condition(reagent name)

- fasta file of the studied RNA with the empty structure[.....]

- shape file conditionShape.txt, it correponds to the reactivity of the condition we would like to see in the final structures.

*****************************************************RNAstruct.Config***************
Parameters to get modified:
-rnafile 
-constraint  i.e: constraints: 1M7,1M7MG,NMIA
- SHAPEVis : colormap used shape file name
- numberofsruct: number of strcutures generqted for each condition, once the value is fixed a folder OutputSamples'numberofsruct' is created.

***********************************************Output*********************************
-a logfile 'Logfile.txt' that contain the caracteristics of clusters (diameter, cumulated Boltzmaan probability, meann distance between strutcures, centroid structures and corresponding energies...)
