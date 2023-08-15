# ERMDS Obfuscation Dataset
## Introduction
Multi-Target Malware Generation (MTMG) is an attack framework designed to target multiple learning-based malware detection systems (LB-MDS) concurrently. Utilizing reinforcement learning, MTMG can orchestrate simultaneous attacks on multiple LB-MDS systems. The framework chooses an obfuscation technique and its relevant parameters from the action space, based on the observed state of the malware. This selection enables the creation of adversarial examples intended to deceive numerous LB-MDS. Comprehensive details are available in our research paper titled "MTMG: A Framework for Generating Adversarial Examples Targeting Multiple Learning-based Malware Detection Systems" (PDF format).

MTMG boasts formidable efficacy against LB-MDS, encompassing commercial antivirus software. When targeting a singular commercial antivirus application, MTMG achieves an impressive attack success rate of over 90%. In scenarios involving multiple such applications, MTMG consistently demonstrates an attack success rate exceeding 80%. To underscore the robust offensive capabilities of MTMG, we are offering access to a malware database. This repository will contain both original malware and versions modified by MTMG, serving as tangible evidence of the tool's efficiency.

**Caution**: Prior to reaching out to us, ensure that you understand and agree with the terms listed below to prevent misuse:

To inquire further, please get in touch with [Lichen Jia](lcjia457@gmail.com). Include your Gmail address in your correspondence so that we can grant you access to the Google Drive folder housing the dataset.

- Sharing Restrictions: Kindly refrain from distributing the data (barring project co-authors). However, we're open to catering to requests from other researchers.

- Usage Intent: Briefly articulate your intended purpose for these binaries. A detailed plan is not mandatory.

- For Academics: If you're affiliated with an academic institution, please use your institutional email for correspondence. Additionally, share a link to a webpage (under the university domain) that confirms your name and affiliation.

- For Industrial Researchers: If you're based in a research lab within the industry, please write to us from your official company email. Introduce yourself and provide background on your organization. Additionally, include a justification letter (PDF format, on official letterhead) elucidating the reasons behind your request for the dataset.

Be advised that any email failing to comply with these stipulations may be disregarded. We will continually update a public directory listing organizations that have been granted access to these samples.

## Download
For researchers who don't require the original malware and MTMG-malware samples, we've extracted features using the [LIEF](https://lief.quarkslab.com/) project (version 0.9.0). These features are consistent with the [Ember](https://github.com/elastic/ember) dataset (details). Every sample is represented as a 2381-feature vector. Access to these feature vectors and sample models is open to everyone. You can download the data from [Google Drive](https://drive.google.com/drive/folders/10Oomg2byEGy3Qiz51MGH7a9sTit1Za-u?usp=sharing).


## Installation
1. Clone this repo from git:

```bash
git clone https://github.com/mtmg-malware/MTMG.git
```

2. We recommend setting up a Python 3.6.9 virtual environment (other Python 3.7 or above versions might also work but didn't test).

```bash
cd MTMG
pip install -r requirements.txt
```

## Evaluating LB-MDS Robustness with MTMG-Malware:
1. Evaluate the robustness of LB-MDS using MTMG-Malware

```bash
python evaluation.py
```

## How to Expand the the Dataset:
To facilitate future researchers in defining their own datasets or expanding the ERMDS dataset, we provide a feature extraction script called feature.py. Modify the paths in this file and run the script to obtain sample features in JSON format.

```bash
python feature.py
```

## Citing
```

```
