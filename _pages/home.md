---
title: Home
layout: splash
permalink: /
date: 2021-12-13T12:00:00-04:00

feature_row:
  - image_path: /assets/images/data.png
    alt: "Data"
    title: "Data"
    excerpt: "Integrated into the data collections featured on MRSHub, browse or contribute datasets used for validating <sup>1</sup>H-MRS processing and quantification pipelines."     
    url: /data/
    btn_label: "Access or submit <sup>1</sup>HMRS-VERI data"
    btn_class: "btn--info btn--small"
  - image_path: /assets/images/forum.png
    alt: "Forum"
    title: "Forum"
    excerpt: "Connect with others in the MRS community about the latest developments in proton MRS data processing and quantification pipeline validation."     
    url: https://forum.mrshub.org/
    btn_label: "To the <sup>1</sup>HMRS-VERI forum on MRSHub"
    btn_class: "btn--info btn--small"
  - image_path: /assets/images/about.png
    alt: "About"
    title: "About"
    excerpt: "Browse papers and other content related to the Proton MRS Validation Effort Resource Initiative."
    url: /about/
    btn_label: "Read more about <sup>1</sup>HMRS-VERI"
    btn_class: "btn--info btn--small"


---

{% capture title-text %}

<sup>1</sup>HMRS-VERI (the Proton MRS Validation Effort Resource Initiative) represents a special endeavor from within the 2021/22 MRS Code and Data Sharing Committee and MRSHub to provide a centralized means to share spectral datasets that can be used to quantitatively validate proton magnetic resonance spectral processing and quantification tools. The tools to be validated include not only those that have already persisted in the literature absent centralized validation efforts but also as-yet agreed upon novel software solutions, open-source and otherwise, that might underlie future consensus recommendations regarding precise and accurate spectral processing and quantification pipelines.

{% endcapture %}

{% capture notice-text %}

<div style="text-align: left">
<strong>Data sets sought for promotion, use, and citation by <sup>1</sup>HMRS-VERI include:</strong><br />
<br />
• <sup>1</sup>H-MRS acquisitions from phantoms, commercial or in-house, of premeasured metabolite concentrations;<br />
• Well defined “gold standard” simulations of metabolite <sup>1</sup>H-MR spectra including simulated and/or measured in vivo-like macromolecule contributions to the baseline and other features that might be exhibited by in vivo spectral datasets, including but not limited to extravoxel lipids, residual water, or lineshape distortions from static field inhomogeneity;<br />
• In vivo <sup>1</sup>H-MR spectral acquisitions from human or other tissues within the context of experiments that also contain supporting measurements of metabolite concentration from non-<sup>1</sup>HMRS experiments, including X-nuclear MRS and/or non-MRS assays;<br />
</div>
<br />
Not sure if your data set belongs here? Want to contribute something more? Email Kelley Swanberg at <a href="mailto:k.swanberg@columbia.edu">k.swanberg@columbia.edu</a>.<br /> 
{% endcapture %}

<div class="notice--info" align="center">
  <h1>Welcome to the Proton MRS Validation Effort Resource Initiative (<sup>1</sup>HMRS-VERI)!</h1>
  {{ title-text | markdownify }}
</div>

<div class="notice--success" align="center">
  {{ notice-text | markdownify }}
</div>

{% include feature_row %}