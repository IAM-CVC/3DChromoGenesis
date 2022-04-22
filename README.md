# 3DChromoGenesis
<!-- [Project](http://iam.cvc.uab.es/portfolio/covair/) | [Arxiv](https://arxiv.org/abs/2005.13928) -->

Chromosome territoriality is not random along the cell cycle, and it is mainly governed by intrinsic chromosome factors and gene expression patterns. Such arrangement is related to the quality of the sperma and, thus, infertility. Up to date, only a few studies have explored the chromosome territoriality during meiosis, most of them limited to specific stages of the process. 
In this study, we have analysed the chromosome positioning in murine spermatogenic cells using a three-dimensionally fluorescence in situ hybridization-based methodology which allows the analysis of the entire karyotype. The main objective of the study was to decipher the radial (from spermatogonia to spermatozoa) and longitudinal (spermatozoa) chromosomal positioning, and the identification of the chromosomal factors that regulate such arrangement. 

To do so, we have developed a specific software to extract a three-dimensional mice model from Fluorescence in situ hybridization (FISH) optical volumes captured with the confocal microscope. Customized developed scripts designed within the Fiji software environment [1] and Matlab R2013b were used to analyse the serial optical images captured with the confocal microscope. Fiji scripts allowed to segment the nuclei and chromosome territories captures in different serial binary images. Matlab scripts allowed to three-dimensionally reconstruct nuclei and the chromosome territories and to extract numerical data that permitted the analysis of the radial positioning of chromosomes and the longitudinal positioning in the case of spermatozoa nuclei. 

<!-- 
## Prerequisites
- Windows, Linux or OSX.
- Matlab 2016a or more.

## Datasets
Download the datasets: 

- `covid-chest-xray`: 152 images of covid19 [covid-chest-xray](https://www.kaggle.com/bachrr/covid-chest-xray). 
- `NIH Chest X-ray Dataset`: 112120 images of 14 Common Thorax Disease Categories [ChestXray-NIHCC](http://academictorrents.com/details/557481faacd824c83fbf57dcf7b6da9383b3235a). 

## Scripts 

The following scripts are included (see the script itself for detailed help about inputs and outputs):

- `ChestNIHCC_Dataset_Extraction.m`: Extraction of ChestXray-NIHCC dataset from excel information (Data_Entry_2017.mat).
- `covidchestxray_Dataset_Extraction.m`: Extraction of covid-chest-xray dataset dataset from excel information (metadata_18_03_2020.xlsx).
- `ClassifierAssessment.m`:  Computes Precision and Recall scores for the samples in Data and classifier defined by W.
- `DefinekFold.m`: Computes NFold partition of Data class-wise. That is, for each class a kfold partition is computed and the final partition is given by ensembling all classes folds.
- `Export2Excel4R.m`: Exports results to excel.

*Important: modify all paths to your local ones

## Experiment

These experiments are disigned to explore capability of classical feature spaces for covid discrimination/early detection in XRAY IA methods: SVM classifier over DCV space on HOG trained to discriminate 4 groups (covid19, pneumonia, infiltrate and no finding). 
(see the script itself for detailed help about inputs and outputs).

- `XRayCovidDiagnosis_Comparison2OtherMths.m`
- `XRayCovidDiagnosis_EarlyDetection.m`
- `XRayCovidDiagnosis_ParameterTunning.m`
- `XRayExploring_DimReductionAssessment.m`
- `SampleInfo2PRLData.m`: Convert data to PLR structure.

*Important: for NIH Chest X-ray Dataset, XRayTest.mat is too large. You can generate it by using SampleInfo2PRLData.m


## Citation
If you use this code for your research, please cite our paper:

```
@misc{gil2020early,
    title={Early Screening of SARS-CoV-2 by Intelligent Analysis of X-Ray Images},
    author={D. Gil and K. Díaz-Chito and C. Sánchez and A. Hernández-Sabaté},
    year={2020},
    eprint={2005.13928},
    archivePrefix={arXiv},
    primaryClass={eess.IV}
}
```


## Acknowledgments

The research leading to these results has received funding from the European Union Horizon 2020 research and
innovation programme under the Marie Sklodowska-Curie grant agreement No 712949 (TECNIOspring PLUS) and
from the Agency for Business Competitiveness of the Government of Catalonia.

This work was supported by Spanish projects RTI2018-095209-B-C21, FIS-G64384969, Generalitat de Catalunya,
2017-SGR-1624, SGR-2017-01597 and CERCA-Programme. Debora Gil is supported by Serra Hunter Fellow. The Titan X Pascal used
for this research was donated by the NVIDIA Corporation.

"Dedicat a la mama (DGil)"
-->
