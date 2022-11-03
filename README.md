# On the Interaction of Regularization Factors in Low-resource Neural Machine Translation
This repository contains the necessay packages and configuration files for our models used for our submission to EAMT 22 "On the Interaction of Regularization Factors in Low-resource Neural Machine Translation"

## Abstract
We explore the roles and interactions of the hyper-parameters governing regularization, and propose a range of values applicable to low-resource neural machine translation.  We demonstrate that default or recommended values for high-resource settings are not optimal for low-resource ones, and that more aggressive regularization is needed when resources are scarce, in proportion to their scarcity.  We explain our observations by the generalization abilities of sharp vs. flat basins in the loss landscape of a neural network.  Results for four regularization factors corroborate our claim: batch size, learning rate, dropout rate, and gradient clipping.  Moreover, we show that optimal results are obtained when using several of these factors, and that our findings generalize across datasets of different sizes and languages.


## Model configuration files
We attach the package requirements for our experiments as well as the configuration files of all models used in the paper in the "configs" folder, inside a folder with the number and name of the section in which they are used. 
In "org_models.ipynb" the model names for each specific section are organized in more detail for each table, with the model's names in order, with an empty line denoting rows.


The abbreviations used in configs folder for the names of the models are as follows:

*bl_10k* - batch size 10'000

*spm_10k* - subword model of 10'000 size (equal for all models)

*dr3* - dropout rate of 0.3

*sf10* - scaling factor of 10

*w16000* - warmup steps of 16'0000

## Reference

Atrio À.R., Popescu-Belis A. (2022) - [On the Interaction of Regularization Factors in Low-resource Neural Machine Translation. Proceedings of the 23rd Annual Conference of the European Association for Machine Translation (EAMT)](https://aclanthology.org/2022.eamt-1.14/).
