# Modular Prosody Tagger
This repository includes the Praat scripts for a modular prosody tagger deployed under the extended Praat  for feature annotations.
An online demo of the tagger is available at http://kristina.taln.upf.edu/praat_web/
A description of the methodology of the tagger can be found in our publication (Domínguez et al.. 2016a) and the specification of Praat on the Web application using a feature vector for annotations in (Dominguez et al., 2016b)

########################
## Requirements
########################

If you want to run the Prosody Tagger scripts found in this repository locally you need to previously download and execute the Extended Praat for feature annotation available in https://github.com/monikaUPF/featureAnnotationforPraat/
That extension for Praat is only available for Linux platforms currently.

########################
## Description
########################

A collection of 8 Praat scripts for the two possible configurations of the tagger are included in this repository. Users can access this tool online clicking on Enter Demo 2 in the main menu of Praat on the Web link mentioned above.
  -  Word Segments: this configuration takes the following 6 modules. This pipeline performs prediction of Prosodic phrases (PPh) boundaries and prominence based on word segmentas and acoustic information.
      -  "mod01.praat" Module 1: Intensity Peak Detection
      -  "mod02.praat" Module 2: Intensity Valley Detection
      -  "mod03.praat" Module 3: Feature Annotation
      -  "mod04.praat" Module 4: Word Segment Export
      -  "mod05a.praat" Module 5: PPh boundary detection (word segments)
      -  "mod06a.praat" Module 6: PPh prominence detection (word segments)
  -  Raw Speech: this configuration takes the following 5 modules and performs prediction of Prosodic phrases boundaries and prominence on computed intensity peaks and valleys
      -  "mod01.praat" Module 1: Intensity Peak Detection
      -  "mod02.praat" Module 2: Intensity Valley Detection
      -  "mod03.praat" Module 3: Feature Annotation
      -  "mod05b.praat" Module 5: PPh boundary detection (raw speech)
      -  "mod06b.praat" Module 6: PPh prominence detection (raw speech)

#####################
## References and citation
#####################

If you use this software or modify the code please cite the following publications:

  - Domínguez, M., M. Farrús and L. Wanner (2016a). An Automatic Prosody Tagger for Spontaneous Speech. Under submission
  - Domínguez, M., I. Latorre, M. Farrús, J. Codina and L. Wanner (2016b). Praat on the Web: An Upgrade of Praat for Semi-Automatic Speech Annotation. Under submission
