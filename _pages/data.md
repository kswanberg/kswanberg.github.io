---
layout: posts
date: 2022-06-27T12:00:00-04:00
title: Data
permalink: /data/
sidebar:
  nav: "data"
---
<br />
## <sup>1</sup>HMRS-VERI Data Types
<br />
This public repository is for sharing spectral datasets that can be used to quantitatively validate proton magnetic resonance spectral processing and quantification tools. The tools to be validated include not only those that have already persisted in the literature absent centralized validation efforts but also as-yet agreed upon novel software solutions, open-source and otherwise, that might underlie future consensus recommendations regarding precise and accurate spectral processing and quantification pipelines. <br />
<br />
Such data sets include the following types:<br />

|         • <sup>1</sup>H-MRS acquisitions from phantoms, commercial or in-house, of premeasured metabolite concentrations;<br />
|         • Well defined “gold standard” simulations of metabolite <sup>1</sup>H-MR spectra including simulated and/or measured in vivo-like macromolecule contributions to the baseline and other features that might be exhibited by in vivo spectral datasets, including but not limited to extravoxel lipids, residual water, or lineshape distortions from static field inhomogeneity;<br />
|         • In vivo <sup>1</sup>H-MR spectral acquisitions from human or other tissues within the context of experiments that also contain supporting measurements of metabolite concentration from non-<sup>1</sup>HMRS experiments, including X-nuclear MRS and/or non-MRS assays;<br />


<br />
## Components of a <sup>1</sup>HMRS-VERI Data Set
<br />
A data set appropriate for submission to <sup>1</sup>HMRS-VERI consists of the following components: 

**1) <sup>1</sup>H-MRS or <sup>1</sup>H-MRSI FIDs** <br />
These might include measurements in a phantom of at least one premeasured metabolite, in vivo measurements supported by non- <sup>1</sup>HMRS concentration estimates of at least one metabolite in the spectrum, simulated spectra or individual metabolites of predetermined and known relative scaling, or composite spectra with simulated metabolites of known predetermined relative scaling plus additional artifacts. For non-simulated, non-composite (i.e., fully measured) data, it is strongly suggested that the submission include trace- and coil-uncombined raw scanner outputs (Siemens, GE, Philips, Agilent/Varian, Bruker, Toshiba). In rare cases non-composite measured data may be preprocessed, but any processing applied must be detailed in the Methodology readme file (details below). Supporting data, like inversion-recovery or echo-time series for relaxivity calculations in the same voxel or imaging data for voxel tissue segmentation, may also be supplied here. Simulated and composite data are expected to include preprocessing that should also be detailed in the Methodology readme text file.

**2) Basis set tailored for use with linear combination model fits to your data**
It is strongly suggested that you supply a full basis set simulated for the exact pulse sequence, including use of the density-matrix formalism with realistic sequence- and vendor-specific pulse shapes, employed in the <sup>1</sup>HMRS acquisitions (or in vivo like metabolite spectral simulations) provided in 1. Freely available basis set simulation tools include [SpinWizard](), [MARSS](), [TARQUIN](), [FID-A](), and others. If you need help simulating a tailored basis set for your potential <sup>1</sup>HMRS-VERI submission please [email us](mailto:kswanberg@@columbia.edu) or post within the <sup>1</sup>HMRS-VERI topic on the [MRSHub Forum](https://forum.mrshub.org/). 

**3) Non- <sup>1</sup>H-MRS concentration estimates for at least one metabolite present in your <sup>1</sup>H-MR spectra.**
As detailed above, estimates of ground-truth metabolite concentrations must derive from a modality other than <sup>1</sup>H-MRS, including premeasurement as in a phantom, predefiniton as in a simulation, or independent supporting measurements as in an in vivo <sup>1</sup>H-MRS data set for which X-nuclear MRS measurements and/or biochemical assay of at least one metabolite concentration within tissue from the same voxel are available. These estimates must be specific to each data set provided, and all procedures pertaining to their derivation must be detailed in the Methodology readme file. 

**4) Methodology readme text file**
This file or group of files, housed together with the other components of your <sup>1</sup>H-MRS data set and provided separately from the `SUBMISSION.md` and `LICENSE.md` summaries submitted for front-end display in the <sup>1</sup>HMRS-VERI data index on MRSHub, should detail the following information about the methods behind your <sup>1</sup>H-MR spectra and supporting data, basis, and ground-truth concentration estimates, based on the [Minimimum Reporting Standards in Magnetic Resonance in Spectroscopy (MRSinMRS)](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/nbm.4484)<sup>1</sup>: 

<sup>1</sup>H-MR spectra:<br />
|   Scanner field strength, manufacturer, model<br />
|   RF coil nuclei (transmit/receive), channel number, type, body part<br /> 
|   Additional hardware used<br />
|   Pulse sequence<br />
|   Volume of Interest (VOI) location(s) (note: for MRSI, 2D/3D, FOV in all directions, matrix size, acceleration factors, sampling method)<br />
|   Nominal VOI size (cm<sup>3</sup>; mm<sup>3</sup>)<br />
|   Repetition time (T<sub>R</sub>); echo time (T<sub>E</sub>); if applicable, mixing time (T<sub>M</sub>); inversion time(s) (T<sub>I</sub>)<br />
|   Number of acquisitions (N<sub>A</sub>) per spectrum (note: for kinetic time series, N<sub>A</sub> per time point, averaging method, and total N<sub>A</sub> over whole series)<br />
|   Spectral width (Hz)<br />
|   Number of spectral points<br />
|   Frequency offsets<br />
|   Water suppression method<br />
|   Shimming method, reference peak, and thresholds for acceptance of shim chosen<br />
|   Triggering or motion correction method<br />
|   If preprocessed, all software and processing steps applied<br />
<br />
Supporting MRI:<br /> 
|   Scanner field strength, manufacturer, model<br />
|   RF coil nuclei (transmit/receive), channel number, type, body part<br /> 
|   Additional hardware used<br />
|   Pulse sequence<br />
|   2D/3D, FOV in all directions, matrix size, acceleration factors, sampling method<br />
|   Nominal VOI size (cm<sup>3</sup>; mm<sup>3</sup>)<br />
|   Repetition time (T<sub>R</sub>); echo time (T<sub>E</sub>); if applicable, inversion time(s) (T<sub>I</sub>)<br />
|   Number of acquisitions (N<sub>A</sub>)<br /> 
<br />
Basis set:<br /> 
|   Software<br />
|   Framework (product-operator; density-matrix)<br />
|   Field strength<br /> 
|   Pulse sequence<br />
|   Repetition time (T<sub>R</sub>); echo time (T<sub>E</sub>); if applicable, mixing time (T<sub>M</sub>); inversion time(s) (T<sub>I</sub>)<br />
|   Pulse shapes (type; scanner vendor or custom)<br />
|   Spectral width (Hz)<br />
|   Number of spectral points<br />
|   ROI size and number of spatial points used for RF simulation<br />
|   Angles used for gradient simulation<br /> 
|   Relaxation considered in lineshape?<br /> 
<br />
Ground-truth concentration estimates:<br /> 


<sup>1</sup> Lin A, Andronesi O, Bogner W, Choi IY, Coello E, Cudalbu C, Juchem C, Kemp GJ, Kreis R, Krššák M, Lee P, Maudsley AA, Meyerspeer M, Mlynarik V, Near J, Öz G, Peek AL, Puts NA, Ratai EM, Tkáč I, Mullins PG; Experts' Working Group on Reporting Standards for MR Spectroscopy. Minimum Reporting Standards for in vivo Magnetic Resonance Spectroscopy (MRSinMRS): Experts' consensus recommendations. NMR Biomed. 2021 May;34(5):e4484. doi: 10.1002/nbm.4484. Epub 2021 Feb 9. PMID: 33559967; PMCID: PMC8647919.
