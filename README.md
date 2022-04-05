# reprotools
This original dataset was obtained at the Providence VA Medical Center on a Siemens 3T Prisma MRI with a 64-channel head coil.

The original dataset is stored here:
A backup copy of the same dataset is also stored here:

A subset of the data will be made available through: (NDA website or brief description of any data-sharing provisions)

Description:  Multi-subject, multi-modal (options:sMRI,fMRI,dMRI,1H MRS,EEG,Behavior). Desrcibe the dataset's broad purpose, e.g., dataset examines valence and inhibitory processing in suicide.

Data were collected across X sessions  (e.g., ses-01=pre-tx, ses-02=immediately post-tx (acute), ses-03=tx endpoint, ses-04=6mo followup)

ses-01 data were funded by
ses-02 data were funded by

====================      Design Changes and Deviations      =======================================================

Stable changes: Describe any stable changes to experimental procedures across the duration of the study (what changed, when, which subjects' data are impacted, e.g., 1 run of task data was added to the imaging protocol starting with subject X, or collection of the Y task was discontinued for subject X and all subsequent subjects.

Isolated deviations: list of procedural deviations impacting single subject e.g.:
sub-XXXX -- has 100 volumes in Run 9 instead of 140 because of a mecahnical problem at the scanner
sub-XXXX -- no X task data was collected for this left-handed subject


====================      Design and Analysis Procedures      =======================================================

func/
-----
Naming and organization of MRI data follows the BIDS standard <references> and reporting the COBIDAS guidelines (Nichols et al., NATURE NEUROSCIENCE VOLUME 20 | NUMBER 3 | MARCH 2017;http://www.humanbrainmapping.org/files/2016/COBIDASreport.pdf)
Sequences:
X Y minute runs of multiband (factor=#) echo planar imaging were collected during the Y task using a (gradient echo, spin echo, etc.) pulse sequence and the following parameters (echo time, repetition time,flip angle,# of volumes,matrix and voxel size,slice orientation). Specify phase encoding direction (e.g. as A/P, L/R, or S/I). Report whether coverage was whole­brain, and whether or not cerebellum and 
brainstem were included. Report any of the following if they are used: parallel imaging (e.g., GRAPPA=2), dummy scans for T1 stabalization, specialized shimming procedures or scanner­side preprocessing (e.g. real-time distortion correction, prospective-motion correction).

Task design references:
The x task was adapted from the original design described in (may have multiple refs)
Unscanned experimental tasks include (task) described in (may have multiple refs)

Describe critical events in task-fMRI behavioral files. 

VARIABLE           EVENT               		  	 USE

WaitForTrigger	   Timestamp marking trigger receipt  	 Correct event timestamps for latency to trigger           
Stim1Onset	   Emotional condition onset 		 Marks start of emotional trial
Stim1RT		   RT to emotional stimulus		 Marks end of emotional trial



eeg/
----
Cap placement was calibrated to (anatomical landmark, e.g., nasion, left and right ears (lowest depression 
between the tragus and the helix, above the tragus)) following the procedure of <insert reference>.

Describe critical task events or triggers included in any behavioral or other eeg files. 

Trigger            Label               Simplified Label

5         Initial Famous Face               FAMOUS
6         Immediate Repeat Famous Face      FAMOUS
7         Delayed Repeat Famous Face        FAMOUS


Defacing
--------
Defacing of MPRAGE T1 images was performed by X after Y. Describe software used for defacing and provide references.
 
Quality Control
---------------
Mriqc was run on sMRI and fMRI datasets. Results of this analysis are in derivatives/mriqc. Learn more about it here: https://mriqc.readthedocs.io/en/latest/
 
Known Issues
------------
N/A


