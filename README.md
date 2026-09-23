# Rapid, unbiased and precise phenotyping using the ALPHA3D pipeline
A pipeline for extracting in a fast and efficient way phenotypic traits. Processing automated and manual landmarks. Calculate precision, bias and accuracy of the pipeline. Apply quantitative genetics method to the dataset.

__Article:__ Unpublished

__Authors:__ Irene Zanandrea<sup>1†</sup> and Kjetil Lysne Voje<sup>1</sup>

__Affiliation:__ <sup>1</sup>Evolution and Paleobiology, Natural History Museum, University of Oslo, 0562, Oslo

__Contact:__ <sup>†</sup>irene.zanandrea@nhm.uio.no

__Journal:__ NA

__Year:__ NA  

__Abstract:__ 
1.	Phenotypic variation is produced through the interactions between genotype and environment. Despite its importance, our ability to characterize phenomes still remains behind our ability to characterize genomes. There is therefore an urgency to develop techniques that enable the rapid and efficient acquisition of high-dimensional phenotypic data. Traditionally landmarks have been collected manually and in two dimensions, but these two phenotyping bottlenecks have recently been addressed by the availability of 3D technologies and the advent of automated landmark-placement methods.
2.	In this study, we introduce the phenomic pipeline Automated Landmarking and Photogrammetry Acquisition in 3D (ALPHA3D) that combines photogrammetry (a fast, portable and cheap way to create 3D models) with automated landmark placement. This highly automated pipeline is designed to rapidly acquire traits. Its speed enables a faster measurement of morphological structures such as the mammalian cranium, including those of polar bears (Ursus maritimus) used in this study. With ALPHA3D, it takes approximately 20 minutes to progress from photographing a skull to obtain a fully automatically annotated 3D model. We assessed the measurement error (imprecision and bias) of ALPHA3D in extracting size (measured as centroid size), and linear measurements. 
3.	The results showed that photographing and making of the 3D model did not contribute significantly to measurement error. Automated landmarking accounted for most of the error introduced by the pipeline but was for the most part negligible relative to the biological (true) variance among the specimens. We quantified imprecision as the pairwise variance between two measurements (σ2), which approximates the relative measurement error. The mean σ2 across all linear distances was found low, at 0.13%. We detect negligible bias for most traits. Lastly we found a strong correlation between P-matrices obtained manually (PML) and automatically (PAL), confirming the close agreement between results from ALPHA3D and from manual landmarking. 
4.	Overall, our results show how ALPHA3D can be used as a rapid, unbiased and precise phenotyping tool to extract morphological traits from mammalian skulls.

__Info:__ This repository contains scripts and data used for analyses in the publication.

__Files__ 

_data –_ in this folder there are the landmarks used in the scripts for the analyses.

_scripts –_ this folder contains the scripts used in the analyses. All scripts are commented for reproducibility purposes.
<ul>
  <li>1_imprecision_log.R runs imprecision (as variance) analysis for the automated pipeline.</li>
  <li>2_bias_log.R runs bias analyses.</li>
  <li>3_variance_ML_vs_AL_ log.R runs imprecision (as variance) between automated and manual landmarking.</li>
  <li>4_inaccuracy_log.R runs inaccuracy analysis (precision plus bias squared) .</li>
  <li>5_cov_matrix_log.R creates phenotypic variance-covariance matrices (P-matrices).</li>
  <li>6_RS_analysis_log.R runs quantitative genetics analyses (Random Skewers).</li>
  <li>7_CS_ANOVA_log.R calculates centroid sizes (CS) and runs nested ANOVAs.</li>
  <li>8_meshdist.R runs the meshdist analysis.</li>
  <li>create_lists_and_dataframe.R create lists and dataframe used in the above scripts</li>
  <li>functions_accuracy.R contains R functions loaded in all the scripts.</li>
  <li>imprecision_2nd_part_pipeline.R runs imprecision analysis for the second half of the automated pipeline.</li>
  <li>landmarks_traits.R specifies the name of traits used in the above scripts.</li>
  <li>libraries.R contains the libraries used in all the scripts.</li>
  <li>list_nested_anova.R specifies the name of traits used in the ANOVA analyses.</li>
</ul>

