# Awesome-Class-Agnostic-Counting

Paper list and performance comparison for **CAC** (Class Agnostic Counting)



## Papers (latest first)
- **[CounTR]** CounTR: Transformer-based Generalised Visual Counting [[paper]](https://arxiv.org/pdf/2208.13721.pdf)
- **[RCC]** Learning to Count Anything: Reference-less Class-agnostic Counting with Weak Supervision [[paper]](https://arxiv.org/pdf/2205.10203.pdf) [[code]](https://github.com/ActiveVisionLab/LearningToCountAnything)
- **[RepRPN-Counter]** Exemplar Free Class Agnostic Counting [[paper]](https://arxiv.org/pdf/2205.14212.pdf) (Ranjan)
- **[SAFECount]** Few-shot Object Counting with Similarity-Aware Feature Enhancement [[paper]](https://arxiv.org/pdf/2201.08959.pdf)
- **[LaoNet**] OBJECT COUNTING: YOU ONLY NEED TO LOOK AT ONE [[paper]](https://arxiv.org/pdf/2112.05993.pdf)
- **[BMNet]** Represent, Compare, and Learn: A Similarity-Aware Framework for Class-Agnostic Counting [[paper]](https://openaccess.thecvf.com/content/CVPR2022/papers/Shi_Represent_Compare_and_Learn_A_Similarity-Aware_Framework_for_Class-Agnostic_Counting_CVPR_2022_paper.pdf) [[code]](https://github.com/flyinglynx/Bilinear-Matching-Network)
- **[VCN]** Vicinal Counting Networks [[paper]](https://openaccess.thecvf.com/content/CVPR2022W/L3D-IVU/papers/Ranjan_Vicinal_Counting_Networks_CVPRW_2022_paper.pdf) (Ranjan)
- **[FamNet]** Learning To Count Everything [[paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Ranjan_Learning_To_Count_Everything_CVPR_2021_paper.pdf) [[code]](https://github.com/cvlab-stonybrook/LearningToCountEverything) (Ranjan)
- **[CFOCNet]** Class-agnostic Few-shot Object Counting [[paper]](https://openaccess.thecvf.com/content/WACV2021/papers/Yang_Class-Agnostic_Few-Shot_Object_Counting_WACV_2021_paper.pdf)
- **[GMN]** Class-Agnostic Counting [[paper]](https://arxiv.org/pdf/1811.00472.pdf)



## Comparison (latest last)

| method         | where      | abstract                                                     | 3-shot                                     |                           | 1-shot                         |              | reference-less (all result below is from RCC) |              |
| -------------- | ---------- | ------------------------------------------------------------ | ------------------------------------------ | ------------------------- | ------------------------------ | ------------ | --------------------------------------------- | ------------ |
|                |            |                                                              | FSC147-Val                                 | FSC147-Test               | FSC147-Val                     | FSC147-Test  | FSC147-Val                                    | FSC147-Test  |
| GMN            | ACCV18     | ????????????CAC???????????????????????????                                |                                            |                           | 29.66/89.81                    | 26.52/124.57 | 39.02/106.06                                  | 37.86/141.39 |
| CFOCNet        | WACV21     | ?????????resnet???????????????????????????+self attention                | 21.19/61.41  (from BMNet)                  | 22.10/112.71 (from BMNet) |                                |              |                                               |              |
| FamNet         | CVPR21     | 3-shot ????????????????????????exemplar??????????????????????????????????????????**??????FSC147?????????** | 23.75/69.07                                | 22.08/99.54               | 26.55/77.01                    | 26.76/110.95 | 32.15/98.7 5                                  | 32.27/131.46 |
| VCN            | CVPRW22    | ?????????????????????????????????+????????????                              | 19.38/60.15                                | 18.17/95.60               |                                |              |                                               |              |
| BMNet          | CVPR22     | ??????????????????+???????????????????????????+?????????????????????               | 15.74/58.53                                | 14.62/91.83               | 17.89/61.12                    | 16.89/96.65  |                                               |              |
| LaoNet         | arxiv21.12 | **1-shot** cnn+transformer?????????????????????????????????             | -                                          | -                         | **17.11/56.81**                    | **15.78/97.15**  |                                               |              |
| SAFECount      | arxiv22.01 | ?????????????????????+????????????????????????????????????                      | 15.28/47.20 (11.60/45.05 cross-validation) | 14.32/85.54               | (13.03/48.77 cross-validation) |              |                                               |              |
| RepRPN-Counter | arxiv22.05 | **Exemplar Free** ??????????????????????????????????????????????????????????????????  |                                            |                           |                                |              | 29.24/98.11                                   | 26.66/129.11 |
| RCC            | arxiv22.05 |  FSC147->FSC133????????????????????????????????????????????????????????????ViT????????????????????????????????????  |                                            |                           |                                |              | 17.49/58.81                                   | 17.12/104.53 |
| CounTR | arxiv22.08 |  ???ViT???MAE????????????cutmix???????????? | **13.13/49.83** | **11.95/91.23** | - | - | **17.40/70.33** | **14.12/108.01** | 
