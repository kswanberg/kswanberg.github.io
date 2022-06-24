---
layout: page
title: About
permalink: /about/
title: ""
header: 
  overlay_image: /assets/images/Logo_words.png
  overlay_filter: rgba(205, 239, 154, 0.30)
---

**About the Proton MRS Validation Effort Resource Initiative (<sup>1</sup>HMRS-VERI)<br/>**
{: style="text-align: center; font-size:1.5em; color: #2a9ebd;"}
<br/>
Despite recent consensus efforts to define field standards for in vivo magnetic resonance spectroscopy (MRS) data acquisition, processing, quantification, and reporting, multiple sources of spectral and absolute quantification error in proton (<sup>1</sup>sup>H) MRS remain incompletely characterized. Consequently, the question remains: What is the most accurate approach to processing, spectrally quantifying, and absolutely quantitating the metabolite concentrations from a given <sup>1</sup>H-MRS data set?<br/>
<br/>
Traditionally this question has been tackled from the perspective of expected or measured variabilities only. Such approaches have centered on methods like comparing estimates of metabolite fit precision by Cramér-Rao Lower Bounds (CRLB), or optimizing spectral quantification steps against coefficients of variation. Many of these approaches, while derived directly from the data in question and often convenient to implement, rely on assumptions that errors are adequately described by Gaussian distributions, eliding distinctions between stochastic imprecisions inherent in imperfect measurements and systematic inaccuracies introduced by imperfect models.<br/>
<br/>
Missing from this puzzle has been a concerted effort to systematize and question the extent to which these assumptions may deviate from the reality of particular data types and processing streams. If, for instance, literature values for water T<sub>2</sub> are systematically low when applied to a particular experimental group relative to control, assessing within-group coefficients of variation will not capture this error. As another example, if the baseline of a spectral fit model is defined with the incorrect stiffness below key metabolite signals thus systematically over- or underestimated across an entire experiment, Cramér-Rao Lower Bounds, based strictly on pointwise Gaussian deviations from an otherwise perfect model, will not capture this error. Alternatively, if a coupling constant or pulse shape underlying metabolite basis function simulation deviates from reality, measurements of Gaussian variability around the mean model solution like CRLB will also fail to capture this error.<br/>
<br/>
The <sup>1</sup>H-MRS community is in need of methods to quantify and communicate such errors against ground-truth standards. The ideal such standard is a data set with a perfectly known solution that is also generalizable to quality conditions seen in the experiment for which validation is being attempted.<br/>
<br/> 
<sup>1</sup>HMRS-VERI represents an effort to collect data that approach this ideal. This includes but may not be limited to the following types:<br/>
<br/>
• Acquisitions from phantoms, commercial or in-house, of premeasured metabolite concentrations;<br/>
<br/>
• Well defined “gold standard” simulations of metabolite spectra, expected macromolecule contributions to the baseline, and other features that might be exhibited by in vivo spectral datasets, including but not limited to extravoxel lipids, residual water, or lineshape distortions from static field inhomogeneity;<br/>
<br/>
• In vivo spectral acquisitions from human or other tissues within the context of experiments that also contain supporting measurements of metabolite concentration from non-MRS assays;<br/>
<br/>
• In vivo acquisitions of signals that do not necessarily include supporting prior knowledge but could be useful to include as nuisance parameters for quantification attempts using the aforementioned simulated standards. An example might be acquired metabolite-nulled (i.e., mostly macromolecule) spectra that can be summed with simulated metabolite resonances to provide baseline shapes similar to those that might be seen in vivo.<br/>
<br/>
Such datasets, linked with the appropriate information regarding their characteristics and limitations, will provide a testing ground for <sup>1</sup>H-MRS data pipelines, particularly preprocessing and spectral quantification procedures, both existing and novel, against standards providing high-quality estimates of ground truth and some degree of generalizability to in vivo application.<br/>
<br/>
Like the complex and conditional pattern of field guidelines published with the recent consensus papers, this effort cannot fully clarify uncertainties surrounding <sup>1</sup>H-MRS measurement and quantification in a single definitive finding. Some sources of error, particularly those introduced by assumed parameters of absolute quantification, will likely not be addressable by quantification against simulated or even measured data sets. Other sources of error, like spectral baseline modeling technique, are bound to exhibit some specificity to the data set at hand and limited generalizability to other types of <sup>1</sup>H-MRS experiment. The goal of this effort is not a simplistic guideline for the single best procedure to derive either relative or absolute metabolite concentrations from <sup>1</sup>H-MR spectra. Rather, this repository of ground-truth datasets provide a foundation for more explicit and rigorous investigation of possible such procedures as currently applied to a variety of 1H-MRS data without the context of quantifiable performance outputs. 

