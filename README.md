# A survey of deep learning and graph neural network for predicting miRNA-disease associations: databases, computational methods, challenges and future directions
![GitHub stars](https://img.shields.io/github/stars/sheng-n/DL_GNN_miRNA_disease_methods?color=red) ![GitHub forks](https://img.shields.io/github/forks/sheng-n/DL_GNN_miRNA_disease_methods?color=green&label=Fork) ![visitors](https://visitor-badge.glitch.me/badge?page_id=sheng-n.DL_GNN_miRNA_disease_methods)

## What is miRNA?
RNA can be divided into two categories based on its coding function: (1) RNAs with coding potential, and (2) RNAs without coding potential, also known as non-coding RNA (ncRNA), which includes microRNAs (miRNA), snoRNAs, circRNAs and lncRNAs. Long non-coding RNAs (lncRNAs) are a major class of important ncRNAs with the lengths more than 200 nucleotides. An increasing number of lncRNA have been found to be abnormally expressed in human diseases, and play a critical role in tumor development.

## Table of Contents
* [Overview](#Overview) 
* [Data resources](#Data-resources) 
  - [LncRNA-disease association data resources](#LncRNA-disease-association-data-resources)
  - [LncRNA-related data resourcess](#LncRNA-related-data-resources)
  - [Disease-related data resources](#Disease-related-data-resources)
* [Deep learning-based methods](#Deep-learning-based-methods) 
  - [Full connected neural network](#Full-connected-neural-network)
  - [Convolutional neural network](#Convolutional-neural-network)
  - [Autoencoder](#Autoencoder)
  - [Generative adversarial network](#Generative-adversarial-network)
* [Graph neural network-based methods](#Graph-neural-network-based-methods) 
  - [Graph feature extraction](#Graph-feature-extraction)
  - [Graph matrix completion](#Graph-matrix-completion)

## Overview
* We collect miRNA- and disease-related databases for MDA prediction, including miRNA-disease association databases, miRNA-related databases, and disease-related databases. 
* We provide the first a comprehensive overview of 45 MDA prediction models based on deep learning and graph neural networks. We classify the two types of models in detail, deep learning models such as autoencoder, multi-layer perceptron, convolutional neural network, variational autoencoder, gated recurrent unit, and generative adversarial network; graph neural network models such as graph convolutional network, graph attention network, graph autoencoder, as shown below figure 1.
![Computational methods](https://user-images.githubusercontent.com/95516781/190976776-7559da50-8787-48c5-836a-043daba949a2.png)

Fig 1: Deep learning and Graph neural network computational methods for MDA prediction. 

## Data resources
### miRNA-disease association data resources
| Database  | Description  | URL | 
|:------------------:|:-----:|:---------------: |
|HMDD v3.2 | Documents 19,166 lncRNAs, 529 diseases and 10,564 association in Homo sapiens, Mus musculus, Rattus norvegicus and Gallus gallus  | http://www.cuilab.cn/hmdd|
|dbDEMC 3.0    |Collects 2,659 lncRNAs, 216 cancers and 9,254 associations in human     |https://www.biosino.org/dbDEMC|
|miR2Disease    |Collects 2,659 lncRNAs, 216 cancers and 9,254 associations in human     |http://www.mir2disease.org/|
|miRCancer   |Collects 2,659 lncRNAs, 216 cancers and 9,254 associations in human     |http://mircancer.ecu.edu/ |
|miRwayD   |Collects 2,659 lncRNAs, 216 cancers and 9,254 associations in human     |http://www.mirway.iitkgp.ac.in/ |
|MNDR v4.0           |Records 39,880 lncRNA, over 1,600 diseases and 295,834 associations in 11 mammals |http://www.rnadisease.org/ |

### miRNA-related data resources
| Database  | Description  | URL | 
|:------------------:|:-----:|:---------------: |
|miRbase v22  | An archive of functional genomics datas  | https://www.mirbase.org/
|mirTarbase    |Records the comprehensive knowledge database of ncRNA from 39 speciesn |https://miRTarBase.cuhk.edu.cn/ |
|miRWalk |Documents ncRNA sequences for 296 species  |http://mirwalk.umm.uni-heidelberg.de/|
|starbase (ENCORI)   |Collects sequence, structure, function and phenotype information of experimentally validated lncRNAs|https://starbase.sysu.edu.cn/|
|lncRNASNP2|Records lncRNA-miRNA, miRNA-mRNA, ncRNA-RNA interactions information| http://bioinfo.life.hust.edu.cn/lncRNASNP|
|miREnvironment    |Documents the regulatory interactions between ncRNAs and other biomolecules|http://www.cuilab.cn/miren|


### Disease-related data resources
| Database  | Description  | URL | 
|:------------------:|:-----:|:---------------: |
|MeSH  | The DO semantically integrates disease and medical vocabularies  | http://www.nlm.nih.gov/ |
|HPO     |A comprehensive logical standard for describing and computationally analyzing phenotypic abnormalities found in human diseases |https://hpo.jax.org/app/ |
|OMIM  |Describes genes with known sequence and phenotypes   |http://www.ncbi.nlm.nih.gov/omim  |
|DisGeNet   |Collects 30,170 diseases, 21,671 genes and 1124,942 associations|https://www.disgenet.org/|
|LncRNADisease|Records 893 diseases, 1,206 miRNAs and 35,547 associations in human| http://www.rnanut.net/lncrnadisease/|

## Deep learning models for predicting MDAs
### Autoencoder
1. **[DeepMDA]** Fu L, Peng Q. A deep ensemble model to predict miRNA-disease association, Scientific Reports 2017;7(1):14482. [**[Download]**](https://www.nature.com/articles/s41598-017-15235-6 "Click") [**[Code]**](https://github.com/gao793583308/NNLDA "Click") 

2. **[DRMLDA]** Zeng M, Lu C, Fei Z et al. DMFLDA: A Deep Learning Framework for Predicting lncRNA–Disease Associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021;18(6):2353-2363. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9054949 "Click") [**[Code]**](https://github.com/CSUBioGroup/DMFLDA "Click")

3. **[MLMDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

4. **[DFELMDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

5. **[MDA-CF]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

6. **[PMDFI]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

7. **[MSCNE]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

8. **[SMALF]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

9. **[MDA-CNN]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

10. **[AEMDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

11. **[iMDA-BN]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

12. **[DANE-MDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

13. **[DBNMDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

14. **[SAEMD]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

15. **[DBMDA]** Zeng M, Lu C, Zhang F et al. SDLDA: lncRNA-disease association prediction based on singular value decomposition and deep learning, Methods 2020;179:73-80. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1046202320300013 "Click") [**[Code]**](https://github.com/CSUBioGroup/SDLDA "Click") 

16. **[VAEMDA]** Su X, You Z, Yi H. Prediction of LncRNA-Disease Associations Based on Network Representation Learning. In: 2020 IEEE International Conference on Bioinformatics and Biomedicine (BIBM). 2020, p.1805-1812. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9313139 "Click") 

17. **[SVAEMDA]** Sheng N, Cui H, Zhang T et al. Attentional multi-level representation encoding based on convolutional and variance autoencoders for lncRNA–disease association prediction, Briefings in Bioinformatics 2020;22(3). [**[Download]**](https://academic.oup.com/bib/article-abstract/22/3/bbaa067/5841901?login=false "Click") 

### Multi-layer perceptron
1. **[EPMDA]** Xuan P, Cao Y, Zhang T et al. Dual Convolutional Neural Networks With Attention Mechanisms Based Method for Predicting Disease-Related lncRNA Genes, Frontiers in genetics 2019;10. [**[Download]**](https://www.frontiersin.org/articles/10.3389/fgene.2019.00416/full "Click") 

2. **[MLRDFM]** Xuan P, Jia L, Zhang T et al. LDAPred: A Method Based on Information Flow Propagation and a Convolutional Neural Network for the Prediction of Disease-Associated lncRNAs, International journal of molecular sciences 2019;20(18). [**[Download]**](https://www.mdpi.com/1422-0067/20/18/4458 "Click") 

### Convolutional neural network 
1. **[CNNDMP]** Xuan P, Sheng N, Zhang T et al. CNNDLP: A Method Based on Convolutional Autoencoder and Convolutional Neural Network with Adjacent Edge Attention for Predicting lncRNA–Disease Associations, International journal of molecular sciences 2019;20(17). [**[Download]**](https://www.mdpi.com/1422-0067/20/17/4260 "Click") 

2. **[CNNMDA]** Zhang Y, Ye F, Xiong D et al. LDNFSGB: prediction of long non-coding rna and disease association using network feature similarity and gradient boosting, BMC Bioinformatics 2020;21(1):377. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-020-03721-0 "Click") [**[Code]**](https://github.com/MLMIP/LDNFSGB "Click") 

3. **[DNRLCNN]** Guo Z-H, You Z-H, Wang Y-B et al. A Learning-Based Method for LncRNA-Disease Association Identification Combing Similarity Information and Rotation Forest, iScience 2019;19:786-795. [**[Download]**](https://www.sciencedirect.com/science/article/pii/S2589004219303086 "Click") 

### Other deep learning methonds
1. **[CEMDA]** Yang Q, Li X. BiGAN: LncRNA-disease association prediction based on bidirectional generative adversarial network, BMC Bioinformatics 2021;22(1):357. [**[Download]**](https://link.springer.com/article/10.1186/s12859-021-04273-7 "Click") [**[Code]**](https://github.com/TomasYang001/BiGAN-lncRNA-disease-associations-prediction "Click")
2. **[GMDA]** Yang Q, Li X. BiGAN: LncRNA-disease association prediction based on bidirectional generative adversarial network, BMC Bioinformatics 2021;22(1):357. [**[Download]**](https://link.springer.com/article/10.1186/s12859-021-04273-7 "Click") [**[Code]**](https://github.com/TomasYang001/BiGAN-lncRNA-disease-associations-prediction "Click")

## Graph neural models for predicting MDAs 
### graph convolutional network
1. **[HGCNMDA(1)]** Xuan P, Pan S, Zhang T et al. Graph Convolutional Network and Convolutional Neural Network Based Method for Predicting lncRNA-Disease Associations, Cells 2019;8(9). [**[Download]**](https://www.mdpi.com/2073-4409/8/9/1012 "Click") 

2. **[Zhu’s method]** Wu Q-W, Xia J-F, Ni J-C et al. GAERF: predicting lncRNA-disease associations by graph auto-encoder and random forest, Briefings in Bioinformatics 2021;22(5). [**[Download]**](https://academic.oup.com/bib/article-abstract/22/5/bbaa391/6067881 "Click") 

3. **[NIMCGCN]** Wu QW, Cao RF, Xia J et al. Extra Trees Method for Predicting LncRNA-Disease Association Based on Multi-layer Graph Embedding Aggregation, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9540266 "Click") [**[Code]**](https://github.com/QingwWu/MLGCNET "Click")

4. **[FCGCNMDA]** Sheng N, Huang L, Wang Y et al. Sheng N, Huang L, Wang Y et al. Multi-channel graph attention autoencoders for disease-related lncRNAs prediction, Briefings in Bioinformatics 2022;23(2). [**[Download]**](https://academic.oup.com/bib/article-abstract/23/2/bbab604/6519791 "Click") [**[Code]**](https://github.com/sheng-n/MGATE "Click")

5. **[MMGCN]** Lan W, Wu X, Chen Q et al. GANLDA: Graph attention network for lncRNA-disease associations prediction, Neurocomputing 2022;469:384-393. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S0925231221011012 "Click") 

6. **[GSCENet]** Xuan P, Zhan L, Cui H et al. Graph Triple-Attention Network for Disease-related LncRNA Prediction, IEEE Journal of Biomedical and Health Informatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9625721 "Click") 

7. **[MDA-GCNFTD]** Silva ABOV, Spinosa EJ. Graph Convolutional Auto-Encoders for predicting novel lncRNA-Disease associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9395216 "Click") 

8. **[MINIMDA]** Silva ABOV, Spinosa EJ. Graph Convolutional Auto-Encoders for predicting novel lncRNA-Disease associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9395216 "Click") 

9. **[HGCNMDA(2)]** Silva ABOV, Spinosa EJ. Graph Convolutional Auto-Encoders for predicting novel lncRNA-Disease associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9395216 "Click") 

10. **[MuCoMid]** Silva ABOV, Spinosa EJ. Graph Convolutional Auto-Encoders for predicting novel lncRNA-Disease associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9395216 "Click") 

11. **[SGNNMD]** Silva ABOV, Spinosa EJ. Graph Convolutional Auto-Encoders for predicting novel lncRNA-Disease associations, IEEE/ACM Transactions on Computational Biology and Bioinformatics 2021:1-1. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9395216 "Click") 

### graph attention network
1. **[HGATMDA]** Wu X, Lan W, Chen Q et al. Inferring LncRNA-disease associations based on graph autoencoder matrix completion, Computational Biology and Chemistry 2020;87:107282. [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S1476927119310114 "Click") 

2. **[GRPAMDA]** Fan Y, Chen M, Pan X. GCRFLDA: scoring lncRNA-disease associations using graph convolution matrix completion with conditional random field, Briefings in Bioinformatics 2021;23(1). [**[Download]**](https://academic.oup.com/bib/article-abstract/23/1/bbab361/6363052?login=false "Click") [**[Code]**](https://github.com/jademyC1221/GCRFLDA "Click")

3. **[HGANMDA]** Zhao X, Zhao X, Yin M. Heterogeneous graph attention network based on meta-paths for lncRNA–disease association prediction, Briefings in Bioinformatics 2021;23(1). [**[Download]**](https://academic.oup.com/bib/article-abstract/23/1/bbab407/6377515?login=false "Click") 

4. **[MDPBMP]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

### graph autoencoder
1. **[GCAEMDA]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

2. **[NIMGSA]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

3. **[GAEMDA]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

4. **[AGAEMD]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

5. **[VGAE-MDA]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

6. **[VGAMD]** Shi Z, Zhang H, Jin C et al. A representation learning model based on variational inference and graph autoencoder for predicting lncRNA-disease associations, BMC Bioinformatics 2021;22(1):136. [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04073-z "Click") [**[Code]**](https://github.com/zhanglabNKU/VGAELDA "Click")

## Welcome to contribute
If you would like to help contribute this list, please feel free to contact me by email:

* Email: shengnan21@mails.jlu.edu.cn
