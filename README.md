# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers which come from the **[SSOAR repository](http://www.ssoar.info/)**. 
This corpus will grow constantly..

## Content
The latest update of files is available in [v3-2018-Mai](https://github.com/exciteproject/ssoar-gold-standard/tree/master/v3-2018-04-24). Other folders are an archive of former files.
* [v3-2018-Mai](v3-2018-Mai)
    1. [pdfs](v3-2018-Mai/1-pdfs)
        * contains selected pdf files.
    2. [layouts](v3-2018-Mai/2-layouts)
        * contains extracted layout files from selected pdfs.
        * **[refext](https://github.com/exciteproject/refext)** is used for layout extraction
    3. [Layout_and_refs_merged_and_checked_by_Anno1](v3-2018-Mai/3-Layout_and_refs_merged_and_checked_by_Anno1)
        * contains layout files with annotated reference strings.
        * reference strings are checked and edited by [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool1)
    4. [References_extracted_from_Layout](v3-2018-Mai/4-References_extracted_from_Layout)
        * contains extracted reference strings from annotated layout files (step 3).
    5. [References_segmented_by_Anno2](v3-2018-Mai/5-References_segmented_by_Anno2).
        * contains segmented reference strings 
        * reference strings are checked and edited by [Annotator Tools](https://github.com/exciteproject/Annotator_tool/tree/master/Annotatortool2).
    6. [Layout_and_segmentated_ref_merged](v3-2018-Mai/6-Layout_and_segmentated_ref_merged)
        * contains a merge of layout and segmented reference strings.

### Selection method
We randomly select our papers from the 33,954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
### Files name
Files name are equal to SSOAR ID (For easier referencing).
> For example, ``12826.pdf`` refers to SSOAR ID 12826.
### How access to papers in SSOAR repository
By searching SSOARID (file name) in [https://www.gesis.org/ssoar/home/](https://www.gesis.org/ssoar/home/), you can access each paper(metadata and pdf).
### Selection criteria
We excluded the following publications from our gold standard:

* Non-German and Non-English publications
* Publications that were in OCR or scanned (images) format.
* Publications that do not contain a reference section.
* Publications that have more than 50 or less than 3 references in their reference section.

A list of excluded papers can be found [here](v3-2018-Mai).