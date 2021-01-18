# FreSaDa: The **Fr**ench **Sa**tire **Da**ta Set

The FreSaDa data set contains regular and satirical samples of text collected from the French news domain.

## 1. License Agreement

**Copyright (C) 2021 - Radu Tudor IONESCU, Adrian Gabriel CHIFU**

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). 

You are free to **share** (copy and redistribute the material in any medium or format) and **adapt** (remix, transform, and build upon the material) under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **NonCommercial** — You may not use the material for commercial purposes.
- **ShareAlike** — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
- **No additional restrictions** — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

## 2. Citation

(to appear)

## 3. Description

#### General Information

FreSaDa, the <i>**Fre**nch **Sa**tire **Da**ta Set</i>, is composed of 11,570  articles  from  the  newsdomain. The news articles are of two types: satirical and regular. Two possible tasks may be considered on FreSaDa:
- Cross-domain binary classification of full news articles into *regular* versus *satirical* examples
- Cross-domain binary classification of headlines into *regular* versus *satirical* examples

The data set is divided into three subsets:
- training (8,716 samples)
- testing (2,854 samples)

Each sample contains the news article's title and text, as well as the corresponding label.

#### Data Organization

The data set is divided in two folders, `train` and `test`, corresponding to the two subsets for training and testing. In each folder there is a subfolder entitled `texts`, containing the texts of the news articles. Each folder also contains a file called `summary.tsv`:

  The `summary.tsv` files contain one sample per row. The format of each row is the following:
  ```
  text_id_1   title_1   label_1
  text_id_2   title_2   label_2
  ...
  text_id_n   title_n   label_n
  ```
  
  where:
  - `text_id` is the filename for the article text (from the `texts` folder)
  - `title` is the article's title
  - `label` is the label for the sample's corresponding class

  The labels are associated as follows:
  -  1 => Satiric News
  - -1 => Regular News
  
  If the experiments require a validation subset, the test subset may be divided into two equal parts: 
  - the first 1,427 samples for validaion
  - the next 1,427 samples for testing
  
## 4. Website

The FreSaDa data set is available at:
[https://github.com/adrianchifu/FreSaDa](https://github.com/adrianchifu/FreSaDa)
