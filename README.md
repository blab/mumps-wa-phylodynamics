# Repeated introductions and intensive community transmission fueled a mumps virus outbreak in Washington State

#### Louise H. Moncla*<sup>1</sup>, Allison Black*<sup>1,2</sup>, Misty Lang<sup>3</sup>, Nicholas R. Graff<sup>3</sup>, Ailyn C. Perez-Osorio<sup>3</sup>, Nicola F. Müller<sup>1</sup>,  Dirk Haselow<sup>4</sup>, Chas DeBolt<sup>3</sup>,Trevor Bedford<sup>1,2</sup>

<sup>1</sup>Fred Hutchinson Cancer Research Center, Seattle, Washington, United States
<sup>1</sup>University of Washington, Seattle, Washington, United States
<sup>3</sup>Office of Communicable Disease Epidemiology, Washington State Department of Health, United States
<sup>4</sup>Arkansas Department of Health, Little Rock, Arkansas, United States

<sup>*</sup>these authors contributed equally to this work 

## Abstract 
In 2016/2017, Washington State experienced a mumps outbreak despite high childhood vaccination rates, with cases more frequently detected among school-aged children and members of the Marshallese community. We sequenced 166 mumps virus genomes collected in Washington and other US states, and traced mumps introductions and transmission within Washington. We uncover that mumps was introduced into Washington approximately 13 times, primarily from Arkansas, sparking multiple co-circulating transmission chains. Although age and vaccination status may have impacted transmission, our dataset could not quantify their precise effects. Instead, the outbreak in Washington was overwhelmingly sustained by transmission within the Marshallese community. Our findings underscore the utility of genomic data to clarify epidemiologic factors driving transmission, and pinpoint contact networks as critical for mumps transmission. These results imply that contact structures and historic disparities may leave populations at increased risk for respiratory virus disease even when a vaccine is effective and widely used.

## Overview
This repo contains all of the code used to perform the analyses for this project tracing mumps transmission during an outbreak in Washington. Sequence data generated for this project can be found [here](https://github.com/blab/mumps-seq/tree/master/data), along with the [protocols and pipelines](https://github.com/blab/mumps-seq) for amplifying and sequencing mumps genomes from buccal swabs. We have deposited all of the raw sequencing reads (with human reads removed) onto the Short Read Archive under Project number [PRJNA641715](https://www.ncbi.nlm.nih.gov/sra/?term=PRJNA641715). Consensus genomes are available in Genbank under accession numbers [MT859507-MT859672](https://www.ncbi.nlm.nih.gov/nuccore/?term=MT859507%3AMT859672%5Baccn%5D). 

Alignments and xml files used for beast analyses are available in the `phylogeography` and `structured-coalescent-analyses` directories. We currently are not able to publish full metadata that links the sequence strain name to age, vaccination status, and Marshallese status. We have therefore removed these metadata fields from the uploaded alignments and xml files and replaced them with generic placeholder text, like `vaccination_status`. If we receive permission from the Department of Health to release this metadata, we will update these files.

Similarly, we have a public metadata file with the date of sample collection, Ct value, specimen type, and vaccination status available [here](https://github.com/blab/mumps-wa-phylodynamics/blob/master/sample-metadata-public-2020-10-06.txt). If we are able to release further metadata, we will update this file with the appropriate fields.

Many of the plotting scripts in this repo require [baltic](https://github.com/evogytis/baltic). I have also included a version of baltic that will work with all of these jupyter notebooks within this repository. 

## Citation
[Moncla et al. 2021. Repeated introductions and intensive community transmission fueled a mumps virus outbreak in Washington State. eLife 10: e66448.](https://doi.org/10.7554/eLife.66448)
