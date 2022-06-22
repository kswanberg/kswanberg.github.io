---
title: Document Center
layout: splash
permalink: /index/
date: 2021-12-01T12:00:00-04:00

feature_row:
  - image_path: /assets/images/software.png
    alt: "Software & Code"
    title: "Software & Code"
    excerpt: "Like the MRSHub code repository, this collects software packages and functions to process, manipulate, analyse, and display MRS data, specifically toward the aim of validation spectral processing and quantification pipelines."
    url: /software
    btn_label: "To the code listing"
    btn_class: "btn--info btn--small"
  - image_path: /assets/images/data.png
    alt: "Data"
    title: "Data"
    excerpt: "Like the MRSHub data repository, this collects MRS datasets used for the purpose of validating processing and quantification pipelines."     
    url: /data
    btn_label: "To the data listing"
    btn_class: "btn--info btn--small"

---

{% capture notice-text %}
Page format based on MRSHub. 

The MRSHub is a curated collection of resources for the analysis of magnetic resonance spectroscopy data. It is maintained by the Committee for MRS Code and Data Sharing of the MR Spectroscopy Study Group of the International Society for Magnetic Resonance in Medicine (ISMRM).

**[MRSHub is actively seeking contributions! If you are interested in advancing open science in MRS, please see the MRSHub User Guide!](https://forum.mrshub.org/t/mrshub-user-guide/7)**
{% endcapture %}

<div class="notice--info" align="center">
  <h1>Welcome to the MRSHub proton MRS validation toolkit sharing platform!</h1>
  {{ notice-text | markdownify }}
</div>

{% include feature_row %}