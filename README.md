Description: 
EnzFIND, a method aiming to identify enzymes that may catalyze an input probe reaction 
based on reaction similarity and substrate flexibility.

Availability:
EnzFIND may be downloaded from sourceforge(http://sourceforge.net/projects/enzfind/). 
The project allows user to initiate on console applications for performing assessment.

Installation:
1.	Unzip EnzFIND.zip 
2.	The unzipped folder contains the following directories
a.	Sample data – sample input reaction file in RXN format
b.	Manual – folder containing file format description document
c.	dynamicLib – placeholder to copy Cdk

Execution:
To run the project from the command line, go to the EnzFind folder and
type the following:

java -Xmx2048M -jar EnzFind.jar 

Include the following arguments:

-i <reaction> Input reaction for simulation (File path in case of RXN format or RSMI smiles)
-r <reaction format> intput reaction format [RSMI, RXN]
-o <output file> output file to write the simulation 
-m <file> Metadata file to be used for simulation [by default sample data will be used]
-f <fingerprint> fingerprint to be used. Default fingerprint is ExtendedFingerprinter

The list of fingerprint keys that can be used for various fingerprints are given below:
Key	->	Value
FP	->	Fingerprint
EXTENDEDFP	->	Extended Fingerprint
ESTATEFP	->	EState Fingerprint
GRAPHONLYFP	->	Graphonly Fingerprint
HYBRIDIZATIONFP	->	Hybridization fingerprint
MACCSFP	->	MACCS Fingerprint
PUBCHEMFP	->	Pubchem Fingerprint
SUBSTRUCTUREFP	->	Substructure Fingerprint


Please refer to EnzFind File Formats.docx for further details of metadata file formats and output file format.


