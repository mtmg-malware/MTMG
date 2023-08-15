# ERMDS Obfuscation Dataset
## Introduction
Multi-Target Malware Generation (MTMG)是一个同时攻击多个learning-based malware detection systems（LB-MDS）的攻击框架，该框架使用leverages reinforcement learning to simultaneously attack multiple LB-MDS. MTMG selects the obfuscation method and its corresponding parameters from the action space based on the observed state of the malware, and then applies them to generate adversarial examples that deceive multiple LB-MDS. Further details can be found in our paper "MTMG: A Framework for Generating Adversarial Examples Targeting Multiple Learning-based Malware Detection Systems" PDF.

## Download
We extract the feature vectors using the [LIEF](https://lief.quarkslab.com/) project (version 0.9.0), the same as the [Ember](https://github.com/elastic/ember) dataset (details can be found [here](https://github.com/elastic/ember/blob/master/ember/features.py)). Each sample is represented as a 2381-feature vector. The feature vectors and example models are open to everyone. Download the data here: [Google Drive](https://drive.google.com/drive/folders/10Oomg2byEGy3Qiz51MGH7a9sTit1Za-u?usp=sharing)
- ERMDS-X: Contains raw features for all samples

We will host the original binaries of malware samples. **To avoid misuse, please read and agree to the following conditions before sending us emails.** Please email [Lichen Jia](lcjia@gmail.com). Also, please include your Gmail address in the body so that we can add you to the Google Drive folder where the dataset is stored.

- Do not share the data with others (except your co-authors for the project). We are happy to share with other researchers based upon their requests.
- Explain in a few sentences your plan to use these binaries. It does not need to be a precise plan.
- If you are in academia, contact us using your institution's email and provide us with a webpage registered at the university domain that contains your name and affiliation.
- If you are in a research (industrial) lab, send us an email from your company's email account and introduce yourself and your company. In the email, please attach a justification letter (in PDF format) in official letterhead. The letter needs to state clearly the reasons why this dataset is being requested.

Please note that an email not following the conditions might be ignored. We will maintain a public list of organizations accessing these samples at the bottom. -->

## Installation
1. Clone this repo from git:

```bash
git clone https://github.com/lcjia94/ERMDS.git
```

2. We recommend setting up a Python 3.6.9 virtual environment (other Python 3.7 or above versions might also work but didn't test).

```bash
cd MTMG
pip install -r requirements.txt
```

## Assessing the Robustness of MDS using ERMDS:
1. Evaluate the robustness of MDS using all datasets from ERMDS-X

```bash
python evaluation.py ALL
```

## How to Expand the ERMDS Dataset:
To facilitate future researchers in defining their own datasets or expanding the ERMDS dataset, we provide a feature extraction script called feature.py. Modify the paths in this file and run the script to obtain sample features in JSON format.

```bash
python feature.py
```

## Citing
```

```
