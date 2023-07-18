[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/)
# Image Guided Translation Dataset
## A large-scale listing dataset of 67,728 actual eBay listing images and titles along with translated german titles

[**Image Guided Translation Dataset**](dataset) is created from 67,728 actual eBay listing (item) images and titles provided by sellers. These listings are taken from different sets of categories like Home & Garden, Consumer Electronics, Toys & Hobbies, Business & Industrial, Musical Instruments and Crafts. Listings are also choosen from a wide varity of sellers and locations to form this heterogeneous dataset suitable to train large multimodals.  

All these listings (items) in this dataset are listed by sellers in eBay United States website and had listing title in english provided by seller at the time of listing. Each of these english language listing titles are then manually translated into german by human translators either by professional translators or via crowd-sourcing.

## Purpose of this Image Guided Translation Dataset
Image Guided Translation Dataset is released to do more research collaboration with many universities. This image-guided translation task is aimed at the generation of item titles in a target language. The task can be addressed as a multisource multimodal translation task, which takes source language listing titles in multiple languages and translates them into the target language, using the visual information as additional context. Multimodal translation involves drawing information from more than one modality, based on the assumption that the additional modalities will contain useful alternative views of the input data. 

This deep collaboration with universities will help eBay to find better solutions for handling challenging translation of polysemous words where listing titles are smaller texts, but a very critical information for eBay pages like search results.

## Dataset contents summary

Here are the summary of contents in Image Guided Translation Dataset:

**Training:**

`Listing Images`: 54,378

`Listing Titles (English & German)`: 54,378

**Test:**

`Listing Images`: 6,696

`Listing Titles (English & German)`: 6,696

**Validation:**

`Listing Images`: 6,652

`Listing Titles (English & German)`: 6,652


## Data format 
Data format in the [TSV mapping file](dataset/listingtitle-image-mappings/listingtitles_with_matched_images.en-de.tsv) having the listing titles and corresponding image mappings:


| Label  | Description |
| ------------- | ------------- |
| project_name  | Name of the project  |
| set_name    | train / test / val to specify whether this data is used |
| image_id    | Listing image id                                       |
| image_file  | Listing image file name in the image data files        |
| source      | Seller provided listing title in english language      |
| target      | Translated listing title in german language            |


## Access to the dataset git repo
Please first install Git Large File Storage by following the below instructions. This step has to be done before the large image data files can be downloaded from the repo.
```
https://help.github.com/articles/installing-git-large-file-storage/
```
Then the repo can be cloned using git clone.
```
git clone git@github.com:eBay/ImageGuidedTranslationDataset.git 
```

## Contact
For any questions or comments, please contact [ImageGuidedTranslationDataset google groups](https://groups.google.com/a/ebay.com/g/imageguidedtranslation).

## License
The data is licensed under the [Creative Commons Attribution-NonCommercial license 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
