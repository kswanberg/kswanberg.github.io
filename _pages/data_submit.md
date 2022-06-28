---
layout: posts
date: 2022-06-27T12:00:00-04:00
title: Contributing to <sup>1</sup>HMRS-VERI
permalink: /data/submit
toc: true
sidebar:
  nav: "data"
---

## Data submission procedure
<sup>1</sup>HMRS-VERI data sets are accessible from a dedicated page on [MRSHub](https://mrshub.org/datasets/).<br />

Please read the [<sup>1</sup>HMRS-VERI guidelines to submission](/data/) for an explanation of the types and necessary components of the data acceptable for this project. 

Once the dataset itself is prepared, its submission to <sup>1</sup>HMRS-VERI consist of two parts: 
<br />

**1) Your `SUBMISSION.md` Markdown file**<br />
This is a description of your submitted data, including a link to the data set itself, also used by any [MRSHub submission](https://mrshub.org/datasets_contribute/). You can download a template `SUBMISSION.md` [here](/assets/SUBMISSION_DATA.md).

| Field | Mandatory? | Description |
| ----  | ---------- | ----------- |
| Developer | Yes | The name(s) you want to credit |
| Name of dataset | Yes | The name of the dataset |
| Abstract | Yes | A brief description of the dataset you contribute |
| Type | Yes | The type of data. We recommend to pick one of these: `svs` (single-voxel MRS) or `mrsi` with either `-phant` (measurements in a phantom), `-in vivo` (in vivo measurements supported by non-1HMRS concentration estimates of at least one metabolite in the spectrum), `-sim` (simulated spectra or individual metabolites), or `-comp` (composite spectra with simulated metabolites and additional artifacts)|
| Format | Yes | The file formats used to store your 1) dataset spectra, 2) associated basis sets/functions, 3) ground truth metabolite values, 4) acquisition and simulation methodology, and 5) any additional information provided |
| Sequence | Yes | The MRS sequence(s) used to 1) acquire the dataset and 2) simulate any associated basis sets/functions |
| Credit | No | Indicate how you would like to be credited for your data - for example, if a certain publication should be cited, or whether you would like to be acknowledged in publications using your data |
| Contact | No | A way you can be contacted: an e-mail address, the website of your lab, your LinkedIn/ResearchGate/Google Scholar page. This information will be made available on MRSHub website, so if you would rather your e-mail not be made public, please do not include |
| Publication | No | A publication you want to associate with the submission |
| URL | Yes | A URL to the data set itself associated with the submission. The data may be hosted externally by the submitter (click [here](https://mrshub.org/datasets_host_organize/) for MRSHub suggestions on hosting frameworks) or on the dedicated [Open Science Framework (OSF) project for <sup>1</sup>HMRS-VERI](https://osf.io/26btq/) (latter preferred). If you choose to host your data on our OSF project, this field should include your OSF account name so that you can be granted access |


**2) A `LICENSE.md` Markdown file**<br />
This is a text file describing the limitations on others' use of your data. As per [MRSHub policy](https://mrshub.org/datasets_contribute/), if this file is not explicitly provided, we will default to a [BSD 3-clause license](https://opensource.org/licenses/BSD-3-Clause).<br />

<br />
Please submit both `SUBMISSION.md` and `LICENSE.md` files as attachments by [email](mailto:k.swanberg@columbia.edu) with the subject line "1HMRS-VERI Data Submission." If you choose to host your data on our OSF project instead of externally, please create an account on the [Open Science Framework](https://osf.io/) and include your account name in the data URL field of your `SUBMISSION.md` file. 


## Data privacy and compliance
Stripping private and protected information from all data sets submitted to <sup>1</sup>HMRS-VERI is the sole responsibility of the parties who submit them. As per MRSHub policy, **We assume no responsibility or liability for data that is improperly de-identified, or shared without institutional permission. Such data will be immediately removed.** <sup>1</sup>HMRS-VERI follows the MRSHub policy on data privacy and compliance, the full text of which is available [here](https://mrshub.org/datasets_privacy/). 