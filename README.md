# Dyslexia MRI FastSurfer and FreeSurfer Processing

This repository contains the code used to process raw structural MRI files from the OpenNeuro dyslexia datasets and extract cortical thickness features for the study.

## Files

- `fastsurfer-segmentation.ipynb`  
  This notebook was used to access and organize the raw structural MRI files from the OpenNeuro datasets, then run FastSurfer GPU-based segmentation to generate cortical surface reconstructions.

- `freesurfer-section (5).ipynb`  
  This notebook was used after segmentation to run FreeSurfer CPU-based processing and extract cortical thickness values from selected left-hemisphere reading and language regions.

## Workflow

The raw structural MRI files were obtained from OpenNeuro datasets `ds003126` and `ds005577`. FastSurfer was first used for GPU-based segmentation and cortical surface reconstruction. FreeSurfer CPU-based tools were then used to extract cortical thickness features from the processed outputs.

The extracted cortical thickness values were later used for ratio calculation, statistical testing, and machine learning classification in the related analysis repository.
