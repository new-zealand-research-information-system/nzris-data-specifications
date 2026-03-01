# NZRIS Label Schemes & Code Sets  

There are several label schemes available in NZRIS allowing for categorisation of data. We have aimed to group these in this folder to provide easy access to classifications.


## Values

### Australian and New Zealand Standard Research Classification (ANZSRC)

Code sets are provided for both the 2008 and 2020 versions of the socio-economic objectives and fields of resesarch. For more information about the classifications, see the [ANZSRC page on the Australian Bureau of Statistics website](https://www.abs.gov.au/statistics/classifications/australian-and-new-zealand-standard-research-classification-anzsrc/latest-release).

* [Type of Activity (2020)](/code-sets-label-schemes/toa-2020.csv)
* [Socio-Economic Objectives (2008)](/code-sets-label-schemes/c-socio-economic-objectives-2008.csv)
* [Socio-Economic Objectives (2020)](/code-sets-label-schemes/seo-2020.csv)
* [Fields of Research (2008)](/code-sets-label-schemes/for.csv)
* [Fields of Research (2020)](/code-sets-label-schemes/for-2020.csv)

### International classfications

* [UN Sustainable Development Goals](/code-sets-label-schemes/sdg.csv)
* [Technology readiness level (ISO 16290:2013)](/code-sets-label-schemes/c-technology-readiness-level.csv)

### New Zealand classfications

* [Vision Mātauranga](/code-sets-label-schemes/c-vision-matauranga.csv)
* [Strategic Programme](/code-sets-label-schemes/c-strategic-programme.csv)

## Format

All labels are captured in a single field per record in the _grants.csv file. The format of the field is as follows:  

•	**Label Value** (e.g. 220302 Electronic information storage and retrieval services)\
•	**pipe delimiter**\
•	**Label Scheme Identifier** (e.g. for-2020)\
•	**pipe delimiter**\
•	**Percentage** (e.g. 25)\
•	**semicolon delimiter** = end of record.  

> **Example**
> 
> ```310803 Plant cell and molecular biology|for-2020|25;310804 Plant > developmental and reproductive biology|for-2020|50;310806 Plant > physiology|for-2020|25;260205 Softwood plantations|seo-2020|30;260506 > Kiwifruit|seo-2020|70```
>   
> In the example above there are three Fields of Research 2020 codes:  
>   
> * *310803 Plant cell and molecular biology (25%)*  
> * *310804 Plant developmental and reproductive biology (50%)*  
> * *310806 Plant physiology (25%)*  
> 
> and two Socio-Economic Objectives 2020 codes:  
>   
> * *260205 Softwood plantations (30%)*  
> * *260506 Kiwifruit (70%)* 

This same format applies to all label schemes and all label schemes can be entered in the same field as a string.  For example Strategic Programme information would be added as follows:  
  
310803 Plant cell and molecular biology|for-2020|25;310804 Plant developmental and reproductive biology|for-2020|50;310806 Plant physiology|for-2020|25;260205 Softwood plantations|seo-2020|30;260506 Kiwifruit|seo-2020|70 **;CoRE Bio Protection Research Centre|c-strategic-programme|**  

Files for each of the label schemes are included in this repository.  The first column of each csv file contains the "Label Value" and the file name includes the "Label Scheme Identifier" (e.g. for-2020 label values.csv).   
