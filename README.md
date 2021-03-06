# Strokes Analysis

## Context

According to the [CDC](https://www.cdc.gov/nchs/fastats/leading-causes-of-death.htm), strokes were the 5th leading cause of death in the US in 2020. Due to its relevance, an investigation was carried out to predict the probability of suffering a stroke based on various characteristics of the patients, such as their age, gender, body mass index, among others. The dataset was taken from fedesoriano's [Stroke Prediction Dataset](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset) on Kaggle. Unfortunately, it is very unbalanced, with only about 4% of stroke-positive records. To correct for this, a rebalancing to have an 85% - 15% proportion (no stroke - had stroke) was applied. Then, a random forest model was used for classification, obtaining an accuracy of 85.39% in the test set. By choosing different classification limits, we can decrease the false negative rate, which is of paramount importance in the context of correctly predicting who is likely to have a stroke. With a limit of 10%, a false negative rate (FNR) of 16.07% and a false positive rate of 42.11% (FPR) can be obtained. Lower limits can further reduce the FNR at the cost of increasing the FPR, for which a cost-benefit study regarding follow up tests, such as MRIs, can be performed.


## Developement

The jupyter notebook [eda.ipynb](dev/eda.ipynb) in which the report was made is contained in the [dev](dev/) folder.

## Results

A report is contained in the [report](report/) folder, both in a [Word](report/strokes_analysis.docx) document as well as a [pdf](report/strokes_analysis.pdf) one. 
A presentation is contained in this same folder both in [PowerPoint](report/strokes_analysis.pptx) and [Excel](report/strokes_analysis.xlsx).

## Details

This project was made mainly as part of a Visualization and Narrative crash course. It's main purpose was to focus on the esthetics and storytelling of the report and presentation rather than optimizing results. For this reason, the values acquired for the FNR and FPR could be considerably improved through different courses of action, also, more exploration on interactions could have been performed, amongst other things.