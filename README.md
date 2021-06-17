# Single_cell analysis report for 2021 class

## About Dengue: What You Need to Know

Dengue viruses are spread to people through the bite of an infected Aedes species (Ae. aegypti or Ae. albopictus) mosquito. These mosquitoes also spread Zika, chikungunya, and other viruses.
Dengue is common in more than 100 countries around the world.
Forty percent of the world’s population, about 3 billion people, live in areas with a risk of dengue. Dengue is often a leading cause of illness in areas with risk.
Each year, up to 400 million people get infected with dengue. Approximately 100 million people get sick from infection, and 22, 000 die from severe dengue.
Dengue is caused by one of any of four related viruses: Dengue virus 1, 2, 3, and 4.  For this reason, a person can be infected with a dengue virus as many as four times in his or her lifetime.
 [source](https://www.cdc.gov/dengue/index.html)

![](./images/denv.png "Dengue Virus")

Dengue virus infection has many manifestations, including asymptomatic symptoms, dengue fever (DF) or more severe forms such as dengue hemorrhagic fever (DHF) and dengue shock syndrome (DSS) in affected individuals. Biomarkers provide a dynamic and effective method for understanding diseases and can be used in observational and analytical epidemiology, randomized clinical trials, screening, diagnosis, and prognosis. When choosing the appropriate  treatment, because the vaccine has not been approved for immunization, the early prognosis is very important for patients who have no warning signs but may develop severe dengue hemorrhagic fever later. Severe reactions of dengue fever include T and B storm cell activation and cytokine apoptosis, hematological abnormalities, and complement activation. Unknown factors such as cytokines and complement can temporarily affect the endothelium and change the barrier function of body fluids causing normal endothelial cells and plasma leakage. The host factors such as complemently activated immune and endothelial cells and their products due to dengue disease can be used as biomarkers for severe dengue fever.[1](https://dx.doi.org/10.1186%2Fs12929-015-0191-6).

Biomarkers for early detection of SD based on molecular features of the patients blood.
**~ Early detection save lives.**

DEG analysis extracted from blood or peripheral blood mononuclear cells (PBMCs).
![](./images/biomarker.png "Dengue Virus")
<div class="images", style="backgrounds-color": "white">

![](https://github.com/Takshan/Single_cell/blob/main/figures/scatterfig.png)

</div>
The data consists of **4** individuals with **Dengue Positive** and **4 Dengue Negative** or Control and therefore has 8 datsets in total.<br> Initial QC of data if of very important as it can help in identifying noises and remove these artifacts that may have adverse effect of the further downstream analysis.
![](https://github.com/Takshan/Single_cell/blob/main/figures/rank_genes_groups_leiden_0_detail_single_cluster_info.png)

The datasets was Standardize  for each same and merged for  the analysis by using **scanpy** package.<br>

Anotation of the genes and custering this highly dimensions data is required to identify groups of cells based on the similarities of the transcripts without any prior knowledge of the labels. Moreover, in most situations we do not even know the number of clusters a priori. The problem is made even more challenging due to the high level of noise (both technical and biological).
<div class="images", style="backgrounds-color": "white">
![](https://github.com/Takshan/Single_cell/blob/main/figures/umap_leiden.png)
</div>
For More Visit [Wiki](https://github.com/Takshan/Single_cell/wiki)

Higly variable genes were identified among the samples for further analysis.
<div class="images", style="backgrounds-color": "white">
![](https://github.com/Takshan/Single_cell/blob/main/figures/filter_genes_dispersion_highly_variable_genes.png)

</div>

