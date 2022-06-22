---
title: Document Center
layout: splash
permalink: /
date: 2021-12-01T12:00:00-04:00

feature_row:
  - image_path: /assets/images/software.png
    alt: "Software & Code"
    title: "Software & Code"
    excerpt: "Integrated into the MRSHub code repository, this collects software packages and functions to process, manipulate, analyse, and display MRS data, specifically toward the aim of validation spectral processing and quantification pipelines."
    url: https://mrshub.org/software/
    btn_label: "To the <sup>1</sup>HMRS-VERI software on MRSHub"
    btn_class: "btn--info btn--small"
  - image_path: /assets/images/forum.png
    alt: "Forum"
    title: "Forum"
    excerpt: "Connect with others in the MRS community about the latest developments in proton MRS data processing and quantification pipeline validation."     
    url: https://forum.mrshub.org/
    btn_label: "To the <sup>1</sup>HMRS-VERI forum on MRSHub"
    btn_class: "btn--info btn--small"
  - image_path: /assets/images/data.png
    alt: "Data"
    title: "Data"
    excerpt: "Integrated into the MRSHub data repository, this collects MRS datasets used for the purpose of validating processing and quantification pipelines."     
    url: https://mrshub.org/datasets/
    btn_label: "To the <sup>1</sup>HMRS-VERI datasets on MRSHub"
    btn_class: "btn--info btn--small"

---

{% capture title-text %}

<sup>1</sup>HMRS-VERI (the Proton MRS Validation Effort Resource Initiative) represents a special endeavor from within the 2021/22 MRS Code and Data Sharing Committee to provide a centralized means to share spectral datasets that can be used to quantitatively validate proton magnetic resonance spectral processing and quantification tools. The tools to be validated include not only those that have already persisted in the literature absent centralized validation efforts but also as-yet agreed upon novel software solutions, open-source and otherwise, that might underlie future consensus recommendations regarding precise and accurate spectral processing and quantification pipelines.

{% endcapture %}

{% capture notice-text %}

<div style="text-align: left">
<h3>Data sets sought by <sup>1</sup>HMRS-VERI include the following types:</h3>
<br />
• Acquisitions from phantoms, commercial or in-house, of premeasured metabolite concentrations;<br />
• Well defined “gold standard” simulations of metabolite spectra, expected macromolecule contributions to the baseline, and other features that might be exhibited by in vivo spectral datasets, including but not limited to extravoxel lipids, residual water, or lineshape distortions from static field inhomogeneity;<br />
• In vivo spectral acquisitions from human or other tissues within the context of experiments that also contain supporting measurements of metabolite concentration from non-MRS assays;<br />
• In vivo acquisitions of signals that do not necessarily include supporting prior knowledge but could be useful to include as nuisance parameters for quantification attempts using the aforementioned simulated standards. An example might be acquired metabolite-nulled (i.e., mostly macromolecule) spectra that can be summed with simulated metabolite resonances to provide baseline shapes similar to those that might be seen in vivo.
</div>
<br />
Not sure if your data set fits here? Want to contribute something more? General questions? Comments? Ideas? Please email Kelley Swanberg at k.swanberg@columbia.edu.<br /> 
{% endcapture %}

<div class="notice--info" align="center">
  <h1>Welcome to the Proton MRS Validation Effort Resource Initiative (<sup>1</sup>HMRS-VERI)!</h1>
  {{ title-text | markdownify }}
</div>
<div class="notice--success" align="center">
  {{ notice-text | markdownify }}
</div>


Page format based on MRSHub. The MRSHub is a curated collection of resources for the analysis of magnetic resonance spectroscopy data. It is maintained by the Committee for MRS Code and Data Sharing of the MR Spectroscopy Study Group of the International Society for Magnetic Resonance in Medicine (ISMRM).

{% include feature_row %}